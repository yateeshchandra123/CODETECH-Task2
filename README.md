# CODETECH-Task2

GOWAPT - Go Web Application Penetration Test
GOWAPT is the younger brother of wfuzz a swiss army knife of WAPT, it allow pentester to perform huge activity with no stress at all, just configure it and it's just a matter of clicks.

How to install
To install gowapt just type:

make
sudo make install

Examples

Scan http://www.example.com and filter all 200 OK requests
gowapt -u "http://www.example.com/FUZZ" -w wordlist/general/common.txt -f "code == 200"
