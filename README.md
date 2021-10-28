#!/usr/bin/python
# -*- coding: UTF-8 -*-

from os import system, name
import itertools
import threading
import time
import sys
import datetime
from base64 import b64decode,b64encode
from datetime import date

expirydate = datetime.date(2021, 10, 29)
#expirydate = datetime.date(2021, 8, 30)
today=date.today()
def hero():

    def chalo():
        done = False
        #here is the animation
        def animate():
            for c in itertools.cycle(['|', '/', '-', '\\']) :
                if done:
                    break
                sys.stdout.write('\rconnecting to server for next colour--------- ' + c)
                sys.stdout.flush()
                time.sleep(0.1)
            sys.stdout.write('\rDone!     ')

        t = threading.Thread(target=animate)
        t.start()

        #long process here
        time.sleep(10)
        done = True

    def chalo1():
        done = False
        #here is the animation
        def animate():
            for c in itertools.cycle(['|', '/', '-', '\\']):
                if done:
                    break
                sys.stdout.write('\rgetting the colour wait --------- ' + c)
                sys.stdout.flush()
                time.sleep(0.1)
            sys.stdout.write('\rDone!     ')

        t = threading.Thread(target=animate)
        t.start()

        #long process here
        time.sleep(20)
        done = True

    def clear():
        # for windows
        if name == 'nt':
            _ = system('cls')
        # for mac and linux(here, os.name is 'posix')
        else:
            _ = system('clear')

    clear()
    y=1
    newperiod=period
    banner='figlet RXCE V 2.0'
    thisway=[2,6,8,11,12,15,16,18,19,20]
    thatway=[1,3,4,5,7,9,10,14,13,17]
    numbers=[]
    i=1
    while(y):
        clear()
        system(banner)
        print("Contact me on telegram @RXCE_HACKER")
        print("Enter ",newperiod," Parity Price :")
        current=input()
        current=int(current)
        chalo()
        print("\n---------Successfully Connected to the server-----------")
        chalo1()
        print("\n---------Successfully got the colour -------------")
        print('\n')
        def getSum(n):
            sum=0
            for digit in str(n):
                sum += int(digit)
            return sum
        if i in thisway:
            m=getSum(current)
            n=int(current)%10
            if((m%2==0 and n%2==0) or (m%2==1 and n%2==1)):
                if current in numbers:
                    print(newperiod+1," : 💥🔴RED🔴💥")
                else:
                    print(newperiod+1," : 💥🟢GREEN🟢💥")
            else:
                if current in numbers:
                    print(newperiod+1," : 💥🟢GREEN🟢💥")
                else:
                    print(newperiod+1," : 💥🔴RED🔴💥")
        if i in thatway:
            m=getSum(current)+1
            n=int(current)%10
            if((m%2==0 and n%2==0) or (m%2==1 and n%2==1)):
                if current in numbers:
                    print(newperiod+1,": 💥💥🟢GREEN🟢💥💥")
                else:
                    print(newperiod+1,": 💥💥🔴RED🔴💥💥")
            else:
                if current in numbers:
                    print(newperiod+1,": 💥💥🟢GREEN🟢💥💥")
                else:
                    print(newperiod+1,": 💥💥🔴RED🔴💥💥")
        i=i+1
        newperiod+=1
        numbers.append(current)
        y=input("Do you want to play : Press 1 and 0 to exit \n")
        if(y==0):
            y=False
        if (len(numbers)>19):
            clear()
            system('figlet Thank you!!')
            print("Play on next specified time!!")
            print("-----------Current Time UP----------")
            sys.exit(" \n \n \n Contact on Telegram @RXCE_HACKER")
            print(numbers)
  



if(expirydate>today):
    now = datetime.datetime.now()
    First = now.replace(hour=10, minute=55, second=0, microsecond=0)
    Firstend = now.replace(hour=11, minute=35, second=0, microsecond=0)
    Second = now.replace(hour=13, minute=55, second=0, microsecond=0)
    Secondend = now.replace(hour=14, minute=35, second=0, microsecond=0)
    Third = now.replace(hour=17, minute=25, second=0, microsecond=0)
    Thirdend = now.replace(hour=18, minute=0, second=0, microsecond=0)
    Final = now.replace(hour=19, minute=55, second=0, microsecond=0)
    Finalend = now.replace(hour=20, minute=35, second=0, microsecond=0)

    if (now>First and now<Firstend):
            period=220
            hero()
    elif(now>Second and now<Secondend):
            period=280
            hero()
    elif(False):
            period=0
            hero()
    elif(True):
            period=0
            hero()
    else:
        banner='figlet RXCE V 2.0'
        print("Hi!! Thanks for buying the hack")
        #print("Hi! thanks for trying our DEMO")
        print("----------Your play time-----------")
        print(" sept 2021, 11:00 AM- 11:30 AM")
        print(" sept 2021, 02:00 PM- 02:30 PM")
        print(" Sept 2021, 05:30 PM- 06:00 PM")
        print(" sept 2021, 08:00 PM- 08:30 PM")
        print("Please play on the given time, and ")
        print("If you think it is an error contact")
        print(" admin on telegram @RXCE_HACKER ")
else:
    banner='figlet RXCE'
    system(banner)
    print("*---------*----------*-------------*----------*")
    print("Your hack has expired--- Please contact")
    print(" on telegram ----@RXCE_HACKER for activating")
    print(" Recharge Amount :        Total limit " )
    print(" 1.     1500 INR -------  15 Day (48 Games Daily ")
    print(" 2.     2000 INR -------  30 Days(1200 Games Daily ")
    print("*---------*----------*-------------*----------*")
    print("Your custom hack can be made request from us.")
    print( "Msg me on telegram @RXCE_HACKER")
