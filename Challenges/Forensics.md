

## Forensics
So in forensic, as name suggests..we need to find something which is hidden.

you need to have a great observation skills for this....(With time this will come)

Lets continue...

these are some common things which should be done on any beginner or basic challenge..(First we aill look into tools then I will show on challenges)

- **strings** This ia linux command..which tells what all text is there inside the file..irrespective of its type..file can be executable,text,image etc..

- **online steganography is https://www.aperisolve.com/**
  
- **online audio decoderhttps://morsecode.world/**

- **exiftool** To understand this Lets take a example.. I have a image..it will have some info..like..dimensions,pixels,author etc etc. So, these are called metadata and each file have some metadata..usually challenges have flags or hint saved in their metadata 

  exiftool is a linux command. To install it ```sudo apt install exiftool ```

- **binwalk | foremost** these 2 are linux tools..let say..I have a file mp3..and I have embedded any file inside it..
so for normal person it will be still a mp3 file..but using binwalk or foremost you can see if there is any file in it

- **headers** so..lets start from basic here.. every thing in pc or digital world is made up of 0 and 1..and the files which are in pc..they are formed using hex numbers(to see the hex bytes of file..use hex editor..example-https://www.onlinehexeditor.com/) if you open the hex of any file then in left side you will see the hex bytes and in right side it shows the file type



![Screenshot 2023-10-11 193432](https://github.com/prem-kumar-verma/CTF/assets/84134833/bf2b9801-fff9-4b2a-84e1-de5365e7cfe7)

![Screenshot 2023-10-11 192945](https://github.com/prem-kumar-verma/CTF/assets/84134833/6c0defdf-3af1-4d5a-b73e-777dffa3989c)



using file command also we can see what acturally it is..

![Screenshot 2023-10-11 193836](https://github.com/prem-kumar-verma/CTF/assets/84134833/f9b7b969-5418-44f1-b06f-f8f3c4df0ad8)


  so there is a term magic headers...every file type have some bytes...which is in its left part of header in image above which represnts the specific [extension](https://en.wikipedia.org/wiki/List_of_file_signatures) of that file....if any digit is missing then the file will be corrupted

  so we will get this type of corrupted file with changed header only and we have have to make it correct to see the content of the file

- **Audio Forensics** (Morse + Spectrogram) some text hidden in audio...spectrogram or morse audio will be given
 
  tools used _ sonic-visualizer
 
  how to install ```sudo apt install sonic-visualizer```

## Steghide: Extract Text Files Embedded in JPG/JPEG Images

Steghide is a powerful tool for extracting text files embedded within JPG or JPEG images. It's particularly useful in situations where a creator may have omitted a password, as Steghide can sometimes work without one. To use Steghide, ensure that you have it installed and simply run it with the target image file. If no password is set, you may find hidden text within the image.

**GitHub:** [Steghide Repository](https://github.com/StefanoDeVuono/steghide)

## zsteg: LSB Extractor for Data Hidden in Images

zsteg is an LSB (Least Significant Bit) extractor that can help you search for hidden information in images. It's particularly effective in challenges involving changes to LSB or MSB (Most Significant Bit). The flag or hidden data may be placed in these bits. zsteg works with various image formats, including PNG and BMP. To use it, install zsteg and run it on your target image file.

**GitHub:** [zsteg Repository](https://github.com/zed-0xff/zsteg.git)

## Stegsolve: View Images in Different Formats

Stegsolve is a Java-based tool that allows you to view images in various formats, from a normal image in black and white to other visual representations. This tool is incredibly handy for examining images in steganography or forensic challenges. To use Stegsolve, run it with a Java command on the image you wish to explore.

**GitHub:** [Stegsolve Repository](https://github.com/e3amn2l/stegsolve)

These tools are valuable assets for digital forensics and cybersecurity professionals seeking to uncover hidden data within images and explore them in different visual formats.


## Stegsnow: Extract Hidden Text from Text Files

Stegsnow is a versatile tool used for extracting concealed text, such as passwords and whitespace text, from text files. It comes in handy when you encounter text files where only visible text is apparent, and copying the entire file reveals hidden whitespace or other content. Stegsnow allows you to unveil these hidden elements, which may contain valuable information, including flags or installation hints.
Find Stegsnow on GitHub at [https://github.com/Paradoxis/Stegsnow](https://github.com/Paradoxis/Stegsnow).

  
## Stegseek: Lightning-Fast Steghide Cracker
Stegseek is a lightning-fast steghide cracker, built as a fork of the original steghide project. It boasts extraordinary speed, capable of processing the entire rockyou.txt* wordlist in under 2 seconds. Additionally, Stegseek can extract steghide metadata without the need for a password, making it an essential tool for uncovering hidden data within files. 
Find Stegseek on GitHub at [https://github.com/RickdeJager/stegseek](https://github.com/RickdeJager/stegseek).

