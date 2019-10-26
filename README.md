# Tools
## Web Exploitation
#### **Burpsuite**
Digunakan untuk testing web security.  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/burpsuite | bash
```

#### **SQLMAP**  
Digunakan untuk SQL Injection.  
**Instalasi :**
```
wget https://raw.githubusercontent.com/miqdadyyy/CTF-Documentation/master/Tools/Web%20Exploitation/sqlmap | bash
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

## Forensic

## Reverse Engineering

## Pwn
