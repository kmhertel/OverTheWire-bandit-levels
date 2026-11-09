# OverTheWire-bandit-levels
Repository containing my experiences, solutions and explanation of completed levels

Level 0 ------
i needed to log into the game using ssh, using the websites provided and the details given with the port, IP, username and password, i determined the inputs needed to be:
ssh -p 2220 bandit0@bandit.labs.overthewire.org
then
password: bandit0

Level 1 ------
had to find the readme ASCII text using the provided (may need) commands on the website, after trying each command followed by "read me", using
cat readme
allowed me to read the text within the readme, however after further investigation:
ls - lists directories
cd - go to home directory
cat - print all contents
file - unknown
du - list current directories, sub directiories and file size
find - find a file 

password: 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
user: bandit1

logging out of the current ssh is by typing "logout"

level 2 ------
ending a bash command - ctrl + d
as the file name is a special character, a different approach was needed compared to level 1
again cat was used to read the content of the file, however, ./- was needed to read the special character to check inside what the password is, so the input:
cat ./-
gave the password: PK8fYLZg2hnHSz83plBL1iEPKdD3QToB

level 3 ------
the filename contains both special characters and spaces, initial struggle to realise the special characters were influencing my commands
to deal with spaces, quoting the filename helps to deal with this, but if it still contains special characters then the .\ is required
input: ./"--spaces in this filename--"
password: 7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
