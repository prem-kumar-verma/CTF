

## Forensics
So in forensic, as name suggests..we need to find something which is hidden.

you need to have a great observation skills for this....(With time this will come)

Lets continue...

these are some common things which should be done on any beginner or basic challenge..(First we aill look into tools then I will show on challenges)

- **strings** This ia linux command..which tells what all text is there inside the file..irrespective of its type..file can be executable,text,image etc..

- **exiftool** To understand this Lets take a example.. I have a image..it will have some info..like..dimensions,pixels,author etc etc. So, these are called metadata and each file have some metadata..usually challenges have flags or hint saved in their metadata 

  exiftool is a linux command. To install it ```sudo apt install exiftool ```

  - **binwalk | foremost** these 
2 are linux tools..let say..I have a file mp3..and I have embedded any file inside it..

so for normal person it will be still a mp3 file..but using binwalk or foremost you can see if there is any file in it

- **headers** so..lets start from basic here.. every thing in pc or digital world is made up of 0 and 1..and the files which are in pc..they are formed using hex numbers(to see the hex bytes of file..use hex editor..example-https://www.onlinehexeditor.com/) if you open the hex of any file then in left side you will see the hex bytes and in right side it shows the file





![Screenshot 2023-10-11 192907](https://github.com/prem-kumar-verma/CTF/assets/84134833/3d438ddd-142b-4ad1-96fc-e647f4e834b3)
![Screenshot 2023-10-11 192945](https://github.com/prem-kumar-verma/CTF/assets/84134833/6c0defdf-3af1-4d5a-b73e-777dffa3989c)

   

    
