# Config


## Git SSH setup
```
ssh-keygen -t ed25519 -C "amresh@gmail.com"
```
```
ssh-add ~/.ssh/id_ed25519
```
```
cat ~/.ssh/id_ed25519.pub
```

```
ssh -T git@github.com
```

## Java using sdkman
```
curl -s "https://get.sdkman.io" | bash
```
```
sdk list java
```
```
sdk install java 24.0.1-amzn
```


## Node using nvm
```sh

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm install node
# nvm install --lts
```


## Bun.sh
` curl -fsSL https://bun.sh/install | bash `


## NvChad
`git clone https://github.com/NvChad/starter ~/.config/nvim && nvim`

## Nerd Font 
https://www.nerdfonts.com/font-downloads



## Java VSCode CP setup
```json
{
  "version": "2.0.0",
  "tasks": [
    {
      "label": "Run Java with Input/Output",
      "type": "shell",
      "command": "javac ${file} && java ${fileBasenameNoExtension} < input.txt > output.txt",
      "group": {
        "kind": "build",
        "isDefault": true
      },
      "problemMatcher": [],
      "detail": "Run Java program using input.txt and save output to output.txt"
    }
  ]
}
```


## Java CP in Sublime
```json
{
    "shell_cmd": "/usr/lib/jvm/java-21-openjdk/bin/javac \"$file\" && /usr/lib/jvm/java-21-openjdk/bin/java \"$file_base_name\" < input.txt > output.txt",
    "working_dir": "${file_path}",
    "selector": "source.java",
    "encoding": "utf-8"
}

```