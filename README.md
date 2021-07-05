# RJ15
'''
program to calculate the least amount of notess needed for a monetary value:-
'''
num=int(input('please enter the monetary value: '))
if num>=2000:
  global d2000
  d2000=num//2000
  rem2000=num%2000
  if rem2000>=500:
    global d500
    d500=rem2000//500
    rem500=rem2000%500
    if rem500>=200:
      global d200
      d200=rem500//200
      rem200=rem500%200
      if rem200>=100:
        global d100
        d100=rem200//100
        rem100=rem200%100
        if rem100>=50:
          global d50
          d50=rem100//50
          rem50=rem100%50
          if rem50>=20:
            global d20
            d20=rem50//20
            rem20=rem50%20
            if rem20>=10:
              global d10
              d10=rem20//10
              rem10=rem20%10
              if rem10>=5:
                global d5
                d5=rem10//5
                rem5=rem10%5
                if rem5>=2:
                  global d2
                  d2=rem5//2
                  rem2=rem5%2
                  if rem2==1:
                    global d1
                    d1=1
                  else:
                    #global d1
                    d1=0
                else:
                  #global d2
                  d2=0
              else:
                #global d5
                d5=0
            else:
              #global d10
              d10=0
          else:
            #global d20
            d20=0
        else:
          #global d50
          d50=0
      else:
        #global d100
        d100=0
    else:
      #global d200
      d200=0
  else:
    #global d500
    d500=0
else:
  #global d2000
  d200=0
print('the number of 2000 rupee notes are:',d2000)
print('the number of 500 rupee notes are:',d500)
print('the number of 200 rupee notes are:',d200)
print('the number of 100 rupee notes are:',d100)
print('the number of 50 rupee notes are:',d50)
print('the number of 20 rupee notes are:',d20)
print('the number of 10 rupee notes are:',d10)
print('the number of 5 rupee notes are:',d5)
print('the number of 2 rupee coins are:',d2)
print('the number of 1 rupee coins are:',d1)
total=d2000+d500+d200+d100+d50+d20+d10+d5+d2+d1
print('total number of notes=',total)

                
