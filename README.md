# CVE-2021-4034
 
This is an exploit created for CVE-2021-4034 meant as a POC. It is based off the info at [https://www.qualys.com/2022/01/25/cve-2021-4034/pwnkit.txt](https://www.qualys.com/2022/01/25/cve-2021-4034/pwnkit.txt).


### How to use it:
- Download the exploit folder. Compile prog.c with `gcc prog.c`
- Go to the GCONV_PATH=. folder and ensure that the "code" file is executable (chmod +x code).
- Go to the "code" folder and compile payload.c with `gcc payload.c -o payload.so -shared -fPIC`
- Note: You'll probably want to change "YOUR_USERNAME" in payload.c if you actually want to see if it works.
- After all of this is set, go back to the main folder, and run the program with `./a.out`.
Note: You can rename this file, a.out is simply the default name from GCC.