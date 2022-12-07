# PYTHON-PROJECT-12211123-
#Topic:Random Password Genrator
import random
import string
def main(plen):
    a="abcdefghijklmnopqrstuvwxyz"
    A="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
    num="0123456789"
    y=string.punctuation
    c=y.replace('<','')
    d=c.replace('>','')
    combine=a+A+num+d
    z=random.sample(combine,plen)
    password="".join(z)
    print("YOUR",plen," character password is:",password)
print("WELCOME TO OUR RANDOM PASSWORD GENRATOR")
while(True):
    plen=int(input("Enter the length of password you want or 0 to end the program: "))
    if plen==0:
        print("YOU EXIT THE PROGRAM.")
        break
    else:
        main(plen)

