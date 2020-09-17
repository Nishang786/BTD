#binary to decimal
while True:
    b = input('enter binary number \n\n')
    if b=='done':quit()
    b=list(b)

    n=0
    g=0

    
    for letter in b:
         n=n+1
         if int(letter) > 1:
             print("write correct value")
             break
         
    n=n-1     
    for l in b:
          if n<0:break
          if l == '0':
               g=g+0
               
          elif l=='1':
               g=g+(2**n)
               
          n=n-1
    print(g)                         

    
