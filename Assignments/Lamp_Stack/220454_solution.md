# Details

Rename this file in the format `yourRollNumber_solution.md` (example, `220000_solution.md`) and submit the solution in the Google form link provided 
*** https://forms.gle/RZtKpFcKfrWrYYxF9 ***


## Your zeroth approach below

Reasoning - The program had a string literal assigned to an int array, so it showed compilation error on execution. Converted the int array to a char array which fixed the problem. The output of the program was-
"The answer of this challenge is output of "man" when run on the terminal, copy the exact output"

Executed the "man" command on Ubuntu's terminal.

```
What manual page do you want?
For example, try 'man man'.
```

---

## Your first approach below (first.txt)

Reasoning - The text file contained only a string that didn't make any sense, so it had to be decryption problem.

Given string- "fgauww qgm vav ujsuc s jglslagf wfujqhlagf gf qgmj gof. Lzw xgddgoafy ak s udmw xgj lzw fwpl hmrrdw: UDSKK gx lzsl AFHML"

The given string had isolated 's' in it. From basic English language knowledge we know that a sentence can contain only isolated 'a' characters.

Code - (in C++)

    string s="fgauww qgm vav ujsuc s jglslagf wfujqhlagf gf qgmj gof. Lzw xgddgoafy ak s udmw xgj lzw fwpl hmrrdw: UDSKK gx lzsl AFHML";

    for(int i=0;i<s.size();i++){
        if(s[i]!=' '){
            if((int)s[i]>=97 && (int)s[i]<123){
                if((((int)s[i]-97)-19)<0){
                    cout<<(char)(((((int)s[i]-97)-18+26)%26)+97);
                }
                else{
                    cout<<(char)(((((int)s[i]-97)-18)%26)+97);
                }
            }
            else if((int)s[i]>=65 && (int)s[i]<91){
                if((((int)s[i]-65)-19)<0){
                    cout<<(char)(((((int)s[i]-65)-18+26)%26)+65);
                }
                else{
                    cout<<(char)(((((int)s[i]-65)-18)%26)+65);
                }
            }
        }
        else{
            cout<<s[i];
        }
    }

```
noicee you did crack a rotation encryption on your own The following is a clue for the next puzzle CLASS of that INPUT
```

---

## Your second approach below (strings.txt)

Reasoning - Lamp_Stack_task had two directories of which one was empty. (question_mark is non empty)

Command -

    find ./question_mark/ -name strings.txt

Used the vim command to read strings.txt.

"8dc2evcCSSc4kUy" had password written beside it so the name of the file that contained this string was the password.

Used grep command to find files containing the found string.

Command - (Current directory - /Lamp_Stack_task/question_mark/Lamp_Stack)

    grep -l "8dc2evcCSSc4kUy" ./*.txt

Output -
1) eleven.txt
2) final.txt

```
A - question_mark/Lamp_Stack/1/5/0/3/strings.txt
Password - eleven.txt
```

---

## Your third approach below (fourth.zip)

Reasoning - Used the grep command to recursively find a file which contained the string "DevOps".

Command -

    grep -nr "DevOps" ./get_in

Location -

    ./get_in/4/2_inner/0.txt

```
DevOps{y0ur3_4w350m3_4nd_0ne_5t3p_c1053r}
```

---


- Name : Himanshu Shekhar
- Roll : 220454
- GitHub username: HimanS1708
- Discord username: Himan_S#5958


## Do not tamper below this line

---

Q29yZSB0ZWFtIGtvIGZha2UgZG8=
