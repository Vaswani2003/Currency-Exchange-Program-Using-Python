def titlescreen () :
  print("\t\t\t\t\tHELLO! WELCOME TO PINNACLE CURRENCY EXCHANGE")
  print("\t\t\t\t\t\tTRANSACTION RECEIPT")
  print("The available currencies for exchange are: \n American Dollar \n Canadian dollar \n Australian Dollar \n Yen \n Euros \n Rupees \n Pound \n Rubble \n Dinar")
  print("\t\t\t\t\t\tDESCRIPTION")

def fixcasing( x ) :      #to remove spaces and make all the letters to lower case
  x = x.replace(' ','')  # removes the space in string; if any 
  x = x.lower()
  return x 

def errorchk( x ) :      # spellchecks provided input
  curnl = [ 'americandollar','canadiandollar','australiandollar','yen','euros','rupees','pound','ruble','dinar']
  if x in curnl :
    return 1
  else :
    return 0

def Adollar(x,y) :        #conversion from american dollar to any other currency
  data = { 'canadiandollar' : 1.49 , 'australiandollar' : 1.43 , 'yen' : 134.19 , 'rupees' : 78.04 , 'dinar' : 145.52,'euros' : 0.9,'ruble' : 56.55,"pound":0.82 }
  for i in data :
    if i == x :
      temp = data[i]

  return y*float(temp)

def Rupees(x,y) :       #conversion from rupees to any other currency
  data = {'canadiandollar' : 0.017 , 'australiandollar' : 0.018 , 'yen' : 1.72 , 'americandollar' : 0.013 , 'dinar' : 1.87,'euros' : 0.013, 'ruble' :0.72,"pound":0.010} 
  for i in data :
    if i == x:
      temp = data[i]
  return y*float(temp)

def Cdollar(x,y):     #conversion from canadian dollar to any other currency
  data={"americandollar":1.01,"australiandollar":1.11,"yen":103.58,"dinar":111.68,"euros":0.73,"ruble":41.44,"rupees":59.81,"pound":0.63}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)
 
def Ausdollar(x,y):   #conversion from australian dollar to any other currency
  data={"americandollar":0.69,"canadiandollar":0.90,"yen":93.53,"dinar":100.85,"euros":0.66,"ruble":37.42,"rupees":54,"pound":0.57}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def Yen(x,y):       #conversion from yen to any other currency
  data={"americandollar":0.01,"canadiandollar":0.01,"australiandollar":0.01,"dinar":1.09,"euros":0.01,"ruble":0.41,"rupees":0.58,"pound":0.0061}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def Euros(x,y):     #conversion from euros to any other currency
  data={"americandollar":1.05,"canadiandollar":1.37,"australiandollar":1.51,"dinar":153.83,"yen":142,"ruble":59.97,"rupees":81.82,"pound":0.86}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def Ruble(x,y):       #conversion from ruble to any other currency
  data={"americandollar":0.017,"canadiandollar":0.022,"australiandollar":0.024,"dinar":2.47,"yen":2.29,"euros":0.016,"rupees":1.32,"pound":0.014}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def Dinar(x,y):       #conversion from algerian to any other currency
  data={"americandollar":3.26,"canadiandollar":4.24,"australiandollar":4.70,"ruble":0.037,"yen":439.38,"euros":3.10,"rupees":253.73,"pound":2.66}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def Pound(x,y):       #conversion from pound to any other currency
  data={"americandollar":1.22,"canadiandollar":1.59,"australiandollar":1.79,"ruble":66,"yen":164.98,"euros":164.98,"rupees":95.27,"dinar":177.89}
  for i in data:
    if i==x:
      temp=data[i]
  return y*float(temp)

def convagain():        #to ask for another input
    op=(input("do you wish to convert your money again?:")).lower()
    if op=="no":
       return 1
    else:
      return 0

def take_input() : #takes input and return currency and amount
  while (1) :
    temp = input('Enter the currency you want to convert: ' )
    currency_1 = fixcasing( temp )
    capital = float(input('Please enter the amount:'))

    temp = input('Enter the currency you want to convert into :')
    currency_2 = fixcasing( temp )

    if errorchk(currency_1) == 1 :
      if errorchk(currency_2) == 1 :
        break 
    else :
      print('Invalid Entry')
  return (currency_1,currency_2,capital)


def currency_conversion( currency_1,currency_2,capital ) :

  if currency_1 == 'americandollar' :
    return Adollar(currency_2,capital)
  
  elif currency_1 == 'rupees' :
   return Rupees(currency_2,capital)
  
  elif currency_1=="canadiandollar":
    return Cdollar(currency_2,capital)
  
  elif currency_1=="australiandollar":
    return Ausdollar(currency_2,capital)
  
  elif currency_1=="yen":
    return Yen(currency_2,capital) 

  elif currency_1=="euros":
    return Euros(currency_2,capital) 
  
  elif currency_1=="ruble":
    return Ruble(currency_2,capital) 
  
  elif currency_1=="pound":
    return Pound(currency_2,capital) 
  
  elif currency_1=="dinar":
    return Dinar(currency_2,capital) 
  
#The main program starts here

from IPython.display import clear_output

titlescreen()

while(1) :

  temp = take_input()
  currency_1 , currency_2, capital = temp[0],temp[1],temp[2]

  final = currency_conversion( currency_1, currency_2, capital )

  print('\n\n\nThe Amount would be',final)

  if convagain() == 0 :
    clear_output()
    titlescreen()
    
  else :
    print('\n\nThank you for using our servives\n\nPlease visit again')
    break  

#end of program
