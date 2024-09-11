# Yara

- [Yara](#yara)
  - [Getting Started](#getting-started)
  - [More Conditions](#more-conditions)
    - [Logic Gates](#logic-gates)
  - [Integration with other Frameworks](#integration-with-other-frameworks)
    - [Cuckoo](#cuckoo)
    - [Python](#python)
    - [LOKI](#loki)
    - [THOR](#thor)
    - [FENRIR](#fenrir)
    - [YAYA](#yaya)

The proprietary language that [Yara (Yet Another Rediculous Acronym)](https://yara.readthedocs.io/en/latest/) uses for rules is fairly trivial to pick up, but hard to master. This is because your rule is only as effective as your understanding of the patterns you want to search for.

Using a Yara rule is simple. Every yara command requires two arguments to be valid, these are:
1) The rule file we create
2) Name of file, directory, or process ID to use the rule for.

Every rule must have a name and condition.

For example, if we wanted to use "myrule.yar" on directory "some directory", we would use the following command:
```bash
yara myrule.yar somedirectory
```

## Getting Started

To make a rule that finds all lowercase, uppercase and camelcase versions of the string "Hello World!" create a new yara file and add the following rule:
```js
rule helloworld_checker {
    strings: 
        $hello_world = "Hello World!"
        $hello_world_lowercase = "hello world!"
        $hello_world_uppercase = "HELLO WORLD!"
     // condition: true // This is the simplest condition   
    condition:
        any of them
}
```

Then create 3 files containing the different strings:
```bash
echo "Hello World!" >> normal.txt && echo "HELLO WORLD!" >> uppercase.txt && echo "hello world!" >> lowercase.txt
```

Now call the rule and the response should include all files containing matching strings that are located in the current directory.

```bash
# Checks current directory
yara helloworld_checker.yar ./ 

# Check specific file
yara helloworld_checker.yar uppercase.txt 
```

## More Conditions

To only match the rule if there are 10 or less occurences of the file you can use the >= operator. Alternatively other operators such as `>`, `<`, `==` and `!=` can be used. 

Example rule:

```js
rule helloworld_checker{
	strings:
		$hello_world = "Hello World!"

	condition:
        #hello_world <= 10
}
```

### Logic Gates
You can also use logic such as `and`, `or`, `nand` etc...

This example rule matches when the string is found in a file of size 10KB:
```js
rule helloworld_checker{
	strings:
		$hello_world = "Hello World!" 
        
        condition:
	        $hello_world and filesize < 10KB 
}
```

## Integration with other Frameworks

### Cuckoo
[Cuckoo Sandbox](https://cuckoosandbox.org/) is an automated malware analysis environment. This module allows you to generate Yara rules based upon the behaviours discovered from Cuckoo Sandbox. As this environment executes malware, you can create rules on specific behaviours such as runtime strings and the like.

### Python
Python's PE module allows you to create Yara rules from the various sections and elements of the Windows Portable Executable (PE) structure.

You can (for example) automate scanning parts of your file directory by integrating Yara with Python. This can be done by importing the `yara module` and the built-in `PE` (Portable Executable Reader) module.

A very basic example of scanning a single file can be as follows:
```python
import yara

# Load your YARA rules
rules = yara.compile(filepath="your_rules.yara")

# Open the file you want to scan
with open("your_file.pe", "rb") as f:
    data = f.read()

# Perform the scan
matches = rules.match(data=data)

# Print the matches
for match in matches:
    print(match)
```

### LOKI
[LOKI](https://github.com/Neo23x0/Loki) is a free open-source IOC (Indicator of Compromise) scanner created/written by Florian Roth.

Based on the GitHub page, detection is based on 4 methods:

1. File Name IOC Check
2. Yara Rule Check (we are here)
3. Hash Check
4. C2 Back Connect Check

There are additional checks that LOKI can be used for which can be found in the [readme](https://github.com/Neo23x0/Loki/blob/master/README.md).

LOKI can be [downloaded](https://github.com/Neo23x0/Loki/releases) and used on both Windows and Linux systems.

### THOR
THOR Lite is Florian's newest multi-platform IOC AND YARA scanner. There are precompiled versions for Windows, Linux, and macOS. A nice feature with THOR Lite is its scan throttling to limit exhausting CPU resources. 

For more information and/or to download the binary, [start here](https://www.nextron-systems.com/thor-lite/). You need to subscribe to their mailing list to obtain a copy of the binary. Note that THOR is geared towards corporate customers. THOR Lite is the free version.


### FENRIR
[FENRIR](https://github.com/Neo23x0/Fenrir) is the 3rd tool created by Neo23x0 (Florian Roth). You guessed it; the previous 2 are named above. The updated version was created to address the issue from its predecessors, where requirements must be met for them to function. Fenrir is a bash script; it will run on any system capable of running bash (nowadays even Windows). 

### YAYA

[YAYA](https://github.com/EFForg/yaya) (Yet Another Yara Automation) was created by the EFF (Electronic Frontier Foundation) and released in September 2020. Based on their website, "YAYA is a new open-source tool to help researchers manage multiple YARA rule repositories. YAYA starts by importing a set of high-quality YARA rules and then lets researchers add their own rules, disable specific rulesets, and run scans of files."