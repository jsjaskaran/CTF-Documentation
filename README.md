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

## Reverse Engineering

## Pwn
