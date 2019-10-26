# **F0rensick**
## **Steganography**
 Some usefull tool for Steganography
 1. Steghide  
    Installation :
    ```
    sudo apt install -y steghide 
    ```
    Useful commands:  
    ```
    steghide info file
    ``` 
    displays info about a file whether it has embedded data or not.  
    ```
    steghide extract -sf file
    ```  
    extracts embedded data from a file
  
 2. Stegsolve  
    installation:  
    get it from : [github](https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve)

    commands:  
    ```
    java -jar stegsolve.jar
    ```
 3. Zsteg  
    zsteg is a tool that can detect hidden data in png and bmp files.  
    to install it :  
    ```
    gem install zsteg
    ```
    The source can be found on [github](https://github.com/zed-0xff/zsteg)

    Useful commands:  
    ```
    zsteg -a file
    ```
    Runs all the methods on the given file
    ```
    zsteg -E file
    ```
    Extracts data from the given payload (example : zsteg -E b4,bgr,msb,xy name.png) 
 4. Exiftool  
    Sometimes important stuff is hidden in the metadata of the image or the file , exiftool can be very helpful to view the metadata of the files.  
    Installation : 
    ```
    sudo apt intall -y exiftool
    ```
    Command : 
    ```
    exiftool file
    ```
 5. Exiv2  
    Similar like Exiftool  
    Installation :  
    ```
    sudo apt install exiv2 
    ```
    Usage :  
    ```
    exiv2 file
    ```
 6. Binwalk  
    Installation : 
    ```
    sudo apt install binwalk
    ```
    Usage :  
    ```
    binwalk file 
    ```
    listing Embedded file
    ```
    binwalk --dd=".* file
    ```
    Extract Embedded file

 7. Foremost  
    Installation :
    ```
    sudo apt intall foremost
    ```
    Usage : 
    ```
    foremost file
    ```
 8. StegCracker  
    relate with steghide for bruteforce steghide passparse.   
    Installation :  
    Required install steghide
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
 