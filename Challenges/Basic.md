# Basic things begineer needs to master
- When CTF organizer give you a binary (download file), always run command ``` file [filename]``` on the binary.
  - File command will determine what type of file are you've downloaded. They will check the magic number or file signature in the binary header.
  - Learn more about file signature at [**here**](https://en.wikipedia.org/wiki/List_of_file_signatures).
  - Some of challenge's creator will confuse you up when they change or remove the extension of a binary. Example, the actual binary is ```binary.jpg``` but they changed it to ```binary.exe```. So, the ctf player will thought that it's a executable file instead of image/jpeg file
- Run ```strings -a [filename]``` to extracts strings in the given binary. Some clues or artifacts can be found in the ```strings``` output
- Base64 is the common encoding used in CTF. Learn about it's characteristics and how to decode it. Some online tools that can help you is this [site](https://www.base64decode.org/). But, the better approach is to decode encoded strings using Linux's terminal. It's because some base64 encoded may a binary file. So, if it's a binary file, online tool like in the link can't provide the decoded binary file. It only can decode strings but not binary file.
    - Example of Linux command for base64 is like this ```echo "[strings of the base64]"``` **|** ```base64 -d```
- Learn about number encoding. Hexadecimal, binary, decimal and also ASCII.
    - You can use this [website](https://www.rapidtables.com/convert/number/ascii-hex-bin-dec-converter.html) to convert your strings to each other.
