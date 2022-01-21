# Rock-Paper-Scissors-Game.py
import random

def main():
    rps = input ('Choose between rock (4), paper (5)  or scissors (6)\n')


    if rps == ('4'):
        print ('You choose rock\n ')
    if rps == ('5'):
        print ('You choose paper\n')
    if rps == ('6'):
        print ('You choose scissors\n')

    print ('Rock...')
    print ('paper...')
    print ('scissors!\n')

    rand = (random.randint(4,6))

    '''Win Statements'''
    if rand  == (4) and rps == ('6'):
        print ('I chose rock.\nI win')
    if rand  == (5) and rps == ('4'):
        print ('I chose paper.\nI win')
    if rand  == (6) and rps == ('5'):
        print ('I choose scissors.\nI win')

    '''User Win Statements'''
    if rand  == (4) and rps == ('5'):
        print ('I chose rock.\nYou win')
    if rand  == (5) and rps == ('6'):
        print ('I chose paper.\nYou win')
    if rand  == (6) and rps == ('4y'):
        print ('I choose scissors.\nYou win')

    '''Draw Statements'''
    if rand  == (4) and rps == ('4'):
        print ('I chose rock.\nWe drew')
    if rand  == (5) and rps == ('5'):
        print ('I chose paper.\nWe drew')
    if rand  == (6) and rps == ('6'):
        print ('I choose scissors.\nWe drew')

while True:
    main()
    if input("\nRepeat the program? (Y/N)").strip().upper() != 'Y':
        break
    
