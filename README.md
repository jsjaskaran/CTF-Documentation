# Tools
## Web Exploitation
### **Burpsuite**
Digunakan untuk testing web security.  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/burpsuite && bash burpsuite
```

### **SQLMAP**  
Digunakan untuk SQL Injection.  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/sqlmap && bash sqlmap
```
**Basic Usage :**  
Scanning :
```
python sqlmap.py -u you_website_url
```
Discover Database :
```
python sqlmap.py -u you_website_url --dbs
```
Discover Table :
```
python sqlmap.py -u you_website_url --tables -D database_name
```
Get Column of a table :
```
python sqlmap.py -u you_website_url --tables -D database_name -T table_name
```
Get Data from a table :
```
python sqlmap.py -u you_website_url --dump -D database_name -T table_name
```

### Dirsearch
Digunakan untuk scanning path dari website  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/dirsearch && bash dirsearch
```
**Basic Usage:**
```
python3 dirsearch.py -u URL
```

### Gitdumper
Digunakan untuk dump .git file  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/gitdumper && bash gitdumper
```
**Basic Usage:**
```
git-dumper.py your_website_url /path/to/dir_output
```

### Nmap
**Instalasi :**
```
sudo apt install nmap
```
**Basic usage :**  
Scanning port :
```
nmap -v -A your_website
```
### Javascript Deobsufator
Digunakan untuk perapian javascript code yang sudah di-obfuscate  
**Url :** [https://lelinhtinh.github.io/de4js/](https://lelinhtinh.github.io/de4js/)

### JWT Translator
Encode dan Decode JWT   
**Url :**
[https://www.jsonwebtoken.io/](https://www.jsonwebtoken.io/)

### Commix
All in one jare
```
git clone https://github.com/commixproject/commix
```

## Forensic

### Steghide  
**Installation :**
```
sudo apt install -y steghide
```
**Basic Usage :**  
displays info about a file whether it has embedded data or not.  
```
steghide info file
```
extracts embedded data from a file
```
steghide extract -sf file
```  
### Stegsolve
**Installation :**
```
[https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve](https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve)

java --jar
```

### Zsteg
zsteg is a tool that can detect hidden data in png and bmp files.

**Installation :**
```
gem install zsteg
```

**Basic Usage :**
Runs all the methods on the given file
```
zsteg -a file
```
Extracts data from the given payload (example : zsteg -E b4,bgr,msb,xy name.png)
```
zsteg -E file
```

### Exiftool
Sometimes important stuff is hidden in the metadata of the image or the file , exiftool can be very helpful to view the metadata of the files.  

**Installation :**
```
sudo apt intall -y exiftool
```
**Basic Usage :**
```
exiftool file
```

### Exiv2
Similar like Exiftool  
**Installation :**
```
sudo apt install exiv2
```
**Usage :**
```
exiv2 file
```

### Foremost
Extract hidden file from file :D  
**Installation :**
```
sudo apt intall foremost
```
**Basic Usage :**
```
foremost file
```

### Binwalk
Extract hidden file  
**Installation :**
```
sudo apt install binwalk
```
**Basic Usage :**  
listing Embedded file
```
binwalk file
```
Extract Embedded file
```
binwalk --dd=".* file
```

### StegCracker
relate with steghide for bruteforce steghide passparse.  
**Installation :**  
> Required install steghide  

```
sudo apt install -y steghide
```
Install StegCrack :
```
pip3 install stegcracker
```
Usage :
```
stegcracker <file> [<wordlist>]
```

## Reverse Engineering

## Pwn

### CTF-Documentation

Following is the list of tools and small description that are used for ***Capture the Flag***

- kali linux
- netdiscover - discovers devices on the network
- nmap - to scan for services and ports on the target system
- nikto - to find out more information about what files, folders and services are actually running on the web server
- dirb(web content scanner) - to look for any hidden directories or files on the server
- wp scan utility (wpscan) - to enumerate and find out what the username is for the site on server and then we can do a dictionary attack and find password
- searchsploit - provides with exploits regarding particular tool or software running on server
- msfconsole(metasploit.com) - searching for exploits regarding particular tool or software
- python - language via which we can write small scripts for e.g to ask for bash shell from server