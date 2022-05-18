import time
import random
from getkey import getkey, keys
from colorama import Fore
from replit import db
import math
import sys
import atexit
from zlvl import *
sys.setrecursionlimit(10000)
def cleara():
  print("{}[2J{}[;H".format(chr(27), chr(27)), end="")
  return
def move_to(row,col):
  print("{}[{};{}H".format(chr(27), row, col), end="")
  return
def hide_cursor():
  print('{}[?25l'.format(chr(27)), end="")
  return
def show_cursor():
  print('{}[?25h'.format(chr(27)), end="")
  return
atexit.register(show_cursor)
def clear():
        print("\033c", end="\033[A")
hide_cursor()
if not 'Money' in db.keys():
        db['Money'] = 0
line1 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
line2 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
line3 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
line4 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
ss = 's-----'
dd = 'd-----'
kk = 'k-----'
ll = 'l-----'
score = 0
ronk = 0
mode = True
idk = False
hi = 1
word = ''
mon = db['Money']
color = Fore.RESET
dif = 0.1
start = 0
stop = 0
v = 0
g = 1
rank = ''
keynum = 0
edited = False
if not 'color1' in db.keys():
        db['color1'] = f'{Fore.WHITE}'
if not 'color2' in db.keys():
        db['color2'] = f'{Fore.WHITE}'
if not 'color3' in db.keys():
        db['color3'] = f'{Fore.WHITE}'
if not 'color4' in db.keys():
        db['color4'] = f'{Fore.WHITE}'
color1 = db['color1']
color2 = db['color2']
color3 = db['color3']
color4 = db['color4']
testline1 = ['-']
testline2 = ['-']
testline3 = ['-']
testline4 = ['-']
testline1a = ['-']
testline2a = ['-']
testline3a = ['-']
testline4a = ['-']
def Play():
        global mode, line1, line2, line3, line4, word, dif, v, start, stop, color, score, hi, ronk, keynum, idk, key1, key2, key3, key4, mon, color1, color2, color3, color4
        cleara()
        if mode == False:
                pick = random.randint(1, 5)
                if pick == 1:
                                line1.append(random.choice(ss))
                                line2.append('-')
                                line3.append('-')
                                line4.append('-')
                elif pick == 2:
                                line1.append('-')
                                line2.append(random.choice(dd))
                                line3.append('-')
                                line4.append('-')
                elif pick == 3:
                                line1.append('-')
                                line2.append('-')
                                line3.append(random.choice(kk))
                                line4.append('-')
                elif pick == 4:
                                line1.append('-')
                                line2.append('-')
                                line3.append('-')
                                line4.append(random.choice(ll))
                else:
                        line1.append('-')
                        line2.append('-')
                        line3.append('-')
                        line4.append('-')
        if mode == True and hi == 1:
                if v != len(testline1):
                        line1.append(testline1[v])
                        line2.append(testline2[v])
                        line3.append(testline3[v])
                        line4.append(testline4[v])
                        v += 1
        elif mode == True and hi == 'Beginning':
                if v != len(song1):
                        line1.append(song1[v])
                        line2.append(song2[v])
                        line3.append(song3[v])
                        line4.append(song4[v])
                        v += 1
        elif mode == True and hi == 'Trial And Error':
                if v != len(songb1):
                        line1.append(songb1[v])
                        line2.append(songb2[v])
                        line3.append(songb3[v])
                        line4.append(songb4[v])
                        v += 1
        elif mode == True and hi == 'Troublesome':
                if v != len(songc1):
                        line1.append(songc1[v])
                        line2.append(songc2[v])
                        line3.append(songc3[v])
                        line4.append(songc4[v])
                        v += 1
        elif mode == True and hi == 'Difficulty Spike':
                if v != len(songd1):
                        line1.append(songd1[v])
                        line2.append(songd2[v])
                        line3.append(songd3[v])
                        line4.append(songd4[v])
                        v += 1
        elif mode == True and hi == 'Underestimate':
                if v != len(songe1):
                        line1.append(songe1[v])
                        line2.append(songe2[v])
                        line3.append(songe3[v])
                        line4.append(songe4[v])
                        v += 1
        elif mode == True and hi == 'Freezeburn':
                if v != len(songf1):
                        line1.append(songf1[v])
                        line2.append(songf2[v])
                        line3.append(songf3[v])
                        line4.append(songf4[v])
                        v += 1
        elif mode == True and hi == 'Upward':
                if v != len(songg1):
                        line1.append(songg1[v])
                        line2.append(songg2[v])
                        line3.append(songg3[v])
                        line4.append(songg4[v])
                        v += 1
        elif mode == True and hi == 'Step Out':
                if v != len(songh1):
                        line1.append(songh1[v])
                        line2.append(songh2[v])
                        line3.append(songh3[v])
                        line4.append(songh4[v])
                        v += 1
        elif mode == True and hi == 'Difficulty Curve':
                if v != len(songi1):
                        line1.append(songi1[v])
                        line2.append(songi2[v])
                        line3.append(songi3[v])
                        line4.append(songi4[v])
                        v += 1
        elif mode == True and hi == 'Nevertheless':
                if v != len(songj1):
                        line1.append(songj1[v])
                        line2.append(songj2[v])
                        line3.append(songj3[v])
                        line4.append(songj4[v])
                        v += 1
        elif mode == True and hi == ':flushed:':
                if v != len(songk1):
                        line1.append(songk1[v])
                        line2.append(songk2[v])
                        line3.append(songk3[v])
                        line4.append(songk4[v])
                        v += 1
        elif mode == True and hi == 'Tutorial':
                if v != len(songl1):
                        line1.append(songl1[v])
                        line2.append(songl2[v])
                        line3.append(songl3[v])
                        line4.append(songl4[v])
                        v += 1
        elif mode == True and hi == 'Sine Wave':
                if v != len(songm1):
                        line1.append(songm1[v])
                        line2.append(songm2[v])
                        line3.append(songm3[v])
                        line4.append(songm4[v])
                        v += 1
        if line1[-1] == 's':
                line1[-1] = f'{color1}s{Fore.RESET}'
        elif line2[-1] == 'd':
                line2[-1] = f'{color2}d{Fore.RESET}'
        elif line3[-1] == 'k':
                line3[-1] = f'{color3}k{Fore.RESET}'
        elif line4[-1] == 'l':
                line4[-1] = f'{color4}l{Fore.RESET}'
        if line1 == []:
                clear()
                rillyronka = math.floor(ronk/6)
                if score >= rillyronka*6:
                        rank = 'S'
                elif score >= rillyronka*5:
                        rank = 'A'
                elif score >= rillyronka*4:
                        rank = 'B'
                elif score >= rillyronka*3:
                        rank = 'C'
                elif score >= rillyronka*2:
                        rank = 'D'
                else:
                        rank = 'F'
                print(f'Finish!\nScore: {score}\nRank: {rank}')
                if hi != 1:
                        db['Money'] += score
                        mon = db['Money']
                line1 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line2 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line3 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line4 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                time.sleep(1)
                v = 0
                print('Press anything to play again.')
                key = getkey()
                Menu()
        move_to(0,0)
        for a in line1:
                print(a, end = '')
        print('')
        for b in line2:
                print(b, end = '')
        print('')
        for c in line3:
                print(c, end = '')
        print('')
        for d in line4:
                print(d, end = '')
        print(f"\nScore: {score}\nPress [Backspace] to exit\n{color}{word}{Fore.RESET}")
        if not 's' in line1[0] and not 'd' in line2[0] and not 'k' in line3[0] and not 'l' in  line4[0]:
                line1.remove(line1[0])
                line2.remove(line2[0])
                line3.remove(line3[0])
                line4.remove(line4[0])
                time.sleep(dif)
                Play()
        if idk == False:
                keynum = 0
                if line1[0] == 's':
                        keynum += 1
                if line2[0] == 'd':
                        keynum += 1
                if line3[0] == 'k':
                        keynum += 1
                if line4[0] == 'l':
                        keynum += 1
                idk = True
        start = time.time()
        key = getkey()
        print('\a')
        stop = time.time()
        totaltime = stop - start
        if 's' in key or 'd' in key or 'k' in key or 'l' in key:
                if key in line1[0] or key in line2[0] or key in line3[0] or key in line4[0]:
                        if totaltime < 0.5:
                                score += 1
                                word = 'Perfect'
                                color = Fore.LIGHTGREEN_EX
                        else:
                                word = 'Late'
                                color = Fore.RED
                else:
                        score -= 1
                        word = 'Bad'
                        color = Fore.RED
        else:
                score -= 1
                word = 'Bad'
                color = Fore.RED
        if key == keys.BACKSPACE:
                clear()
                rank = 'N/A'
                print(f'Finish!\nScore: {score}\nRank: {rank}')
                line1 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line2 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line3 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                line4 = ['-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-','-']
                time.sleep(1)
                v = 0
                print('Press anything to play again.')
                key = getkey()
                Menu()
        if score < 0:
                score = 0
        if keynum > 1:
                if 's' in key:
                        line1[0] = '-'
                elif 'd' in key:
                        line2[0] = '-'
                elif 'k' in key:
                        line3[0] = '-'
                elif 'l' in key:
                        line1[0] = '-'
                else:
                        line1.remove(line1[0])
                        line2.remove(line2[0])
                        line3.remove(line3[0])
                        line4.remove(line4[0])
                if keynum == 1:
                        idk = False
                ronk += 1
                keynum -= 1
                Play()
        else:
                line1.remove(line1[0])
                line2.remove(line2[0])
                line3.remove(line3[0])
                line4.remove(line4[0])
                idk = False
                ronk += 1
                Play()
def EditorMaker():
        global testline1, testline2, testline3, testline4, testline1a, testline2a, testline3a, testline4a, g, edited, eee
        clear()
        print('Level Editor\n')
        for a in testline1a:
                print(a, end = '')
        print('')
        for b in testline2a:
                print(b, end = '')
        print('')
        for c in testline3a:
                print(c, end = '')
        print('')
        for d in testline4a:
                print(d, end = '')
        print(f'\n\nPress "s, d, k, l" to place notes.\nCapatalize "s, d, k, l" to put them on the same line.\nPress "backspace" to erase notes.\nPress "space" to leave a space empty.\nPress "enter" to save and quit.\nPress "E" to delete everything.\nPart Limit: {g}/999')
        key = getkey()
        if key == 's':
                if g == 999:
                        clear()
                        print(f'{Fore.RED}Maximum length reached!{color}')
                        time.sleep(1)
                        EditorMaker()
                testline1.append('s')
                testline2.append('-')
                testline3.append('-')
                testline4.append('-')
                testline1a.append('s')
                testline2a.append('-')
                testline3a.append('-')
                testline4a.append('-')
                if g >= 30:
                        testline1a.pop(0)
                        testline2a.pop(0)
                        testline3a.pop(0)
                        testline4a.pop(0)
                g += 1
        elif key == 'd':
                if g == 999:
                        clear()
                        print(f'{Fore.RED}Maximum length reached!{color}')
                        time.sleep(1)
                        EditorMaker()
                testline1.append('-')
                testline2.append('d')
                testline3.append('-')
                testline4.append('-')
                testline1a.append('-')
                testline2a.append('d')
                testline3a.append('-')
                testline4a.append('-')
                if g >= 30:
                        testline1a.pop(0)
                        testline2a.pop(0)
                        testline3a.pop(0)
                        testline4a.pop(0)
                g += 1
        elif key == 'k':
                if g == 999:
                        clear()
                        print(f'{Fore.RED}Maximum length reached!{color}')
                        time.sleep(1)
                        EditorMaker()
                testline1.append('-')
                testline2.append('-')
                testline3.append('k')
                testline4.append('-')
                testline1a.append('-')
                testline2a.append('-')
                testline3a.append('k')
                testline4a.append('-')
                if g >= 30:
                        testline1a.pop(0)
                        testline2a.pop(0)
                        testline3a.pop(0)
                        testline4a.pop(0)
                g += 1
        elif key == 'l':
                if g == 999:
                        clear()
                        print(f'{Fore.RED}Maximum length reached!{color}')
                        time.sleep(1)
                        EditorMaker()
                testline1.append('-')
                testline2.append('-')
                testline3.append('-')
                testline4.append('l')
                testline1a.append('-')
                testline2a.append('-')
                testline3a.append('-')
                testline4a.append('l')
                if g >= 30:
                        testline1a.pop(0)
                        testline2a.pop(0)
                        testline3a.pop(0)
                        testline4a.pop(0)
                g += 1
        if len(testline1a) > 0:
                if key == 'S':
                        testline1[-1] = 's'
                        testline1a[-1] = 's'
                elif key == 'D':
                        testline2[-1] = 'd'
                        testline2a[-1] = 'd'
                elif key == 'K':
                        testline3[-1] = 'k'
                        testline3a[-1] = 'k'
                elif key == 'L':
                        testline4[-1] = 'l'
                        testline4a[-1] = 'l'
        if key == keys.BACKSPACE:
                if testline1 == []:
                        pass
                else:
                        testline1.pop()
                        testline2.pop()
                        testline3.pop()
                        testline4.pop()
                        testline1a.pop()
                        testline2a.pop()
                        testline3a.pop()
                        testline4a.pop()
                        if g >= 31:
                                testline1a.insert(0, testline1[g-31])
                                testline2a.insert(0, testline2[g-31])
                                testline3a.insert(0, testline3[g-31])
                                testline4a.insert(0, testline4[g-31])
                        g -= 1
        elif key == keys.SPACE:
                if g == 999:
                        clear()
                        print(f'{Fore.RED}Maximum length reached!{color}')
                        time.sleep(1)
                        EditorMaker()
                testline1.append('-')
                testline2.append('-')
                testline3.append('-')
                testline4.append('-')
                testline1a.append('-')
                testline2a.append('-')
                testline3a.append('-')
                testline4a.append('-')
                if g >= 30:
                        testline1a.pop(0)
                        testline2a.pop(0)
                        testline3a.pop(0)
                        testline4a.pop(0)
                g += 1
        elif key == keys.ENTER:
                if edited == False:        
                        name = input('Enter a name for your level: ')
                        if name in db['sLevels']['1']:
                                print('You have a level with that name already!')
                                time.sleep(1)
                                EditorMaker()
                        if not 'sLevels' in db.keys():
                                db['sLevels'] = {
                                        1: [],
                                        2: [],
                                        3: [],
                                        4: [],
                                        5: [],
                                        6: []
        }
                        db['sLevels']['1'].append(name)
                        db['sLevels']['2'].append(testline1)
                        db['sLevels']['3'].append(testline2)
                        db['sLevels']['4'].append(testline3)
                        db['sLevels']['5'].append(testline4)
                        db['sLevels']['6'].append(g)
                else:
                        db['sLevels']['2'][eee] = testline1
                        db['sLevels']['3'][eee] = testline2
                        db['sLevels']['4'][eee] = testline3
                        db['sLevels']['5'][eee] = testline4
                        db['sLevels']['6'][eee] = g
                print('Saving...')
                db['list1'] = '-'
                db['list2'] = '-'
                db['list3'] = '-'
                db['list4'] = '-'
                db['list1a'] = '-'
                db['list2a'] = '-'
                db['list3a'] = '-'
                db['list4a'] = '-'
                db['g'] = g
                db['list1'] = ''.join(testline1)
                db['list2'] = ''.join(testline2)
                db['list3'] = ''.join(testline3)
                db['list4'] = ''.join(testline4)
                db['list1a'] = ''.join(testline1a)
                db['list2a'] = ''.join(testline2a)
                db['list3a'] = ''.join(testline3a)
                db['list4a'] = ''.join(testline4a)
                testline1a = ['-']
                testline2a = ['-']
                testline3a = ['-']
                testline4a =  ['-']
                time.sleep(0.25)
                print('Saved!')
                time.sleep(1)
                EditorMenu()
        elif key == "E":
                testline1 = ['-']
                testline2 = ['-']
                testline3 = ['-']
                testline4 = ['-']
                testline1a = ['-']
                testline2a = ['-']
                testline3a = ['-']
                testline4a =  ['-']
                g = 1
        EditorMaker()
def EditorMenu():
        global start, g, testline1, testline2, testline3, testline4, testline1a, testline2a, testline3a, testline4a, eee, edited
        clear()
        print('Level Editor\n')
        print('(1) Edit Level\n(2) Play Level\n(3) Back')
        key = getkey()
        if key == '1':
                clear()
                print('(1) New Level\n(2) Created Levels\n(3) Delete Level\n(4) Back')
                key = getkey()
                if key == '1':
                        g = 1
                        db['g'] = 1
                        EditorMaker()
                if key == '2':
                        clear()
                        print('Created Levels: ')
                        v = 1
                        for i in db['sLevels']['1']:
                                print(f'({v}) {i}')
                                v += 1
                        lvlinpt = input('Which level would you like to edit? ')
                        lvlinpt = lvlinpt.strip()
                        try:
                                lvlinpt = int(lvlinpt)
                                lvlinpt -= 1
                        except ValueError:
                                print('Undefined Level!')
                                time.sleep(1)
                                EditorMenu()
                        if lvlinpt < v and lvlinpt > -1:
                                testline1a = db['sLevels']['2'][lvlinpt]
                                testline2a = db['sLevels']['3'][lvlinpt]
                                testline3a = db['sLevels']['4'][lvlinpt]
                                testline4a = db['sLevels']['5'][lvlinpt]
                                g = db['sLevels']['6'][lvlinpt]
                                edited = True
                                eee = lvlinpt 
                                EditorMaker()
                        else:
                                print('Undefined Level!')
                                time.sleep(1)
                                EditorMenu()
                if key == '3':
                        clear()
                        print('Created Levels: ')
                        v = 1
                        for i in db['sLevels']['1']:
                                print(f'({v}) {i}')
                                v += 1
                        lvlinpt = input('Which level would you like to delete? ')
                        lvlinpt = lvlinpt.strip()
                        try:
                                lvlinpt = int(lvlinpt)
                                lvlinpt -= 1
                        except ValueError:
                                print('Undefined Level!')
                                time.sleep(1)
                                EditorMenu()
                        if lvlinpt < v and lvlinpt > -1:
                                db['sLevels']['1'].pop(lvlinpt)
                                db['sLevels']['2'].pop(lvlinpt)
                                db['sLevels']['3'].pop(lvlinpt)
                                db['sLevels']['4'].pop(lvlinpt)
                                db['sLevels']['5'].pop(lvlinpt)
                                db['sLevels']['6'].pop(lvlinpt)
                                EditorMenu()
                        else:
                                print('Undefined Level!')
                                time.sleep(1)
                                EditorMenu()
                if key == '4':
                        EditorMenu()
        elif key == '2':
                clear()
                print('Created Levels: ')
                v = 1
                for i in db['sLevels']['1']:
                        print(f'({v}) {i}')
                        v += 1
                lvlinpt = input('Which level would you like to play? ')
                lvlinpt = lvlinpt.strip()
                try:
                        lvlinpt = int(lvlinpt)
                        lvlinpt -= 1
                except ValueError:
                        print('Undefined Level!')
                        time.sleep(1)
                        EditorMenu()
                if lvlinpt < v and lvlinpt > -1:
                        testline1 = ['-']
                        testline2 = ['-']
                        testline3 = ['-']
                        testline4 = ['-']
                        testline1a = ['-']
                        testline2a = ['-']
                        testline3a = ['-']
                        testline4a = ['-']
                        for i in db['sLevels']['2'][lvlinpt]:
                                testline1.append(i)
                        for i in db['sLevels']['3'][lvlinpt]:
                                testline2.append(i)
                        for i in db['sLevels']['4'][lvlinpt]:
                                testline3.append(i)
                        for i in db['sLevels']['5'][lvlinpt]:
                                testline4.append(i)
                        Play()
                else:
                        print('Undefined Level!')
                        time.sleep(1)
                        EditorMenu()
        elif key == '3':
                Menu()
        else:
                EditorMenu()
def Menu():
        global start, mode, dif, ss, dd, kk, ll, color, bb, hi, score, ronk, rillywonka, key1, key2, key3, key4, mon, levels, color1, color2, color3, color4
        score = 0
        ronk = 0
        rillywonka = 0
        color = Fore.RESET
        if not 'list1' in db.keys():
                db['list1'] = ''
        if not 'list2' in db.keys():
                db['list2'] = ''
        if not 'list3' in db.keys():
                db['list3'] = ''
        if not 'list4' in db.keys():
                db['list4'] = ''
        if not 'list1a' in db.keys():
                db['list1a'] = ''
        if not 'list2a' in db.keys():
                db['list2a'] = ''
        if not 'list3a' in db.keys():
                db['list3a'] = ''
        if not 'list4a' in db.keys():
                db['list4a'] = ''
        if not 'g' in db.keys():
                db['g'] = 0
        if not 'levels' in db.keys():
                db['levels'] = [['Tutorial', 'Easy'], ['Upward', 'Easy'], ['Beginning', 'Easy'], ['Step Out', 'Medium'], ['Smiley Face', 'Medium'], ['Trial And Error', 'Medium'], [':flushed:', 'Hard'], ['Sine Wave', 'Hard'], ['Difficulty Curve', 'Hard'], ['Troublesome', 'Hard'], ['Difficulty Spike', 'Difficult'], ['Underestimate', 'Difficult'], ['Freezeburn', 'Insane'], ['Nevertheless', 'Insane']]
                levels = db['levels']
        if not 'color' in db.keys():
                db['color'] = [['Red', f'{Fore.RED}']]
                color = db['color']
        if not 'sLevels' in db.keys():
                db['sLevels'] = {
                        1: [],
                        2: [],
                        3: [],
                        4: [],
                        5: [],                                             6: []
}
        clear()
        print(f"""{Fore.BLUE}██████╗ ██╗  ██╗██╗   ██╗████████╗██╗  ██╗███╗   ███╗██╗ ██████╗
██╔══██╗██║  ██║╚██╗ ██╔╝╚══██╔══╝██║  ██║████╗ ████║██║██╔════╝
██████╔╝███████║ ╚████╔╝    ██║   ███████║██╔████╔██║██║██║     
██╔══██╗██╔══██║  ╚██╔╝     ██║   ██╔══██║██║╚██╔╝██║██║██║     
██║  ██║██║  ██║   ██║      ██║   ██║  ██║██║ ╚═╝ ██║██║╚██████╗
╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝      ╚═╝   ╚═╝  ╚═╝╚═╝     ╚═╝╚═╝ ╚═════╝\n██╗    ██╗██████╗ ██╗████████╗██╗███╗   ██╗ ██████╗ 
██║    ██║██╔══██╗██║╚══██╔══╝██║████╗  ██║██╔════╝ 
██║ █╗ ██║██████╔╝██║   ██║   ██║██╔██╗ ██║██║  ███╗
██║███╗██║██╔══██╗██║   ██║   ██║██║╚██╗██║██║   ██║
╚███╔███╔╝██║  ██║██║   ██║   ██║██║ ╚████║╚██████╔╝
 ╚══╝╚══╝ ╚═╝  ╚═╝╚═╝   ╚═╝   ╚═╝╚═╝  ╚═══╝ ╚═════╝ {color}\n""")
        print(f'{Fore.LIGHTYELLOW_EX}Money:{Fore.RESET} {mon}\n')
        print(color1)
        print('(1) Play\n(2) Level Editor\n(3) Difficulty\n(4) Shop\n(5) Color Keys\n')
        key = getkey()
        if key == '1':
                clear()
                print('(1) Maps\n(2) Endless\n(3) Back\n')
                key = getkey()
                if key == '1':
                        hi = 0
                        mode = True
                        bb = False
                        clear()
                        levels = db['levels']
                        v = 0
                        for i in levels:
                                print(f'({v}) {i[0]} - {i[1]}')
                                v += 1
                        print('(Enter) Back')
                        key = input('What level would you like to play? ')
                        try:
                                key = int(key)
                                if key > -1 and key <= v:
                                        hi = levels[key][0]
                                        clear()
                                        print('Get Ready!')
                                        time.sleep(1)
                                        Play()
                        except:
                                pass
                        if key == keys.BACKSPACE:
                                Menu()
                if key == '2':
                        hi = 0
                        mode = False
                        bb = True
                        Play()
                if key == '3':
                        Menu()
        if key == '2':
                hi = 1
                mode = True
                bb = False
                EditorMenu()
        if key == '3':
                clear()
                print(f'What difficulty would you like for endless mode?\n\n(1) Easy\n(2) Medium\n(3) Hard\n(4) Insane\n(5) Catastrophic\n(6) Death Wish')
                key = getkey()
                if key == '1':
                        dif = 0.1
                        ss = 's-----'
                        dd = 'd-----'
                        kk = 'k-----'
                        ll = 'l-----'
                        Menu()
                if key == '2':
                        dif = 0.08
                        ss = 's----'
                        dd = 'd----'
                        kk = 'k----'
                        ll = 'l----'
                        Menu()
                if key == '3':
                        dif = 0.06
                        ss = 's---'
                        dd = 'd---'
                        kk = 'k---'
                        ll = 'l---'
                        Menu()
                if key == '4':
                        dif = 0.04
                        ss = 's--'
                        dd = 'd--'
                        kk = 'k--'
                        ll = 'l--'
                        Menu()
                if key == '5':
                        dif = 0.02
                        ss = 's-'
                        dd = 'd-'
                        kk = 'k-'
                        ll = 'l-'
                        Menu()
                if key == '6':
                        dif = 0.01
                        ss = 's'
                        dd = 'd'
                        kk = 'k'
                        ll = 'l'
                        Menu()
                else:
                        Menu()
        if key == '4':
                clear()
                print(f'The Shop\n\n{Fore.LIGHTYELLOW_EX}Money:{Fore.RESET} {mon}\n')
                if not 'shop' in db.keys():
                        db['shop'] = [[['Pico-8', 'Medium'], 350], [['Blue-Key', f'{Fore.BLUE}'], 500], [['Aeiou', 'Medium'], 500], [['Elttab Dad', 'Hard'], 1120], [['Sine.wav', 'Difficult'], 770], [['Rush E', 'Insane'], 1580]]
                v = 1
                shop = db['shop']
                for i in shop:
                        print(f'({v}) {i[0][0]}: {i[0][1]} - {i[1]}')
                        v += 1
                print('(Backspace) Back')
                key = getkey()
                try:
                        key = int(key)
                        key -= 1
                        if mon >= shop[key][1] :
                                if key < v and key > 0:
                                        db['Money'] >= shop[key][1]
                                        db['Money'] -= shop[key][1]
                                        mon = db['Money']
                                        db['shop'].remove(db['shop'][key])
                                        print('Purchase Success!')
                                        if 'Key' in key:
                                                db['color'].append(shop[key][0])
                                        else:
                                                db['levels'].append(shop[key][0])
                                        time.sleep(0.75)
                except:
                        Menu()
                if key == keys.BACKSPACE:
                        Menu()
                Menu()
        if key == '5':
                clear()
                v = 1
                for i in db['color']:
                        print(f'({v}) {i[0]}')
                        v += 1
                print('(Backspace) Back')
                key = getkey()
                try:
                        key = int(key)
                        key -= 1
                        if key <= v and key >= 0:
                                print('(1) s')
                                print('(2) d')
                                print('(3) k')
                                print('(4) l')
                                print('What key would you like to equip it on?')
                                key = getkey()
                                if key == '1':
                                        db['color1'] = db['color'][1][1]
                                        color1 = db['color1']
                                elif key == '2':
                                        db['color2'] = db['color'][2][1]
                                        color2 = db['color2']
                                elif key == '3':
                                        db['color3'] = db['color'][3][1]
                                        color3 = db['color3']
                                elif key == '4':
                                        db['color4'] = db['color'][4][1]
                                        color4 = db['color4']
                                else:
                                        print('Invalid!')
                                        time.sleep(0.75)
                except:
                        Menu()
                if key == keys.BACKSPACE:
                        Menu()
                Menu()
        if key == '6':
                # Secret way for me to make levels quickly
                lolomg = input('Enter the magic word: ')
                if lolomg == 'addlvl':
                        omg1 = ''
                        omg2 = ''
                        omg3 = ''
                        omg4 = ''
                        for ele in testline1: 
                                omg1 += '"'
                                omg1 += ele  
                                omg1 += '",'
                        for ele in testline2: 
                                omg2 += '"'
                                omg2 += ele  
                                omg2 += '",'
                        for ele in testline3: 
                                omg3 += '"'
                                omg3 += ele  
                                omg3 += '",'
                        for ele in testline4: 
                                omg4 += '"'
                                omg4 += ele  
                                omg4 += '",'
                        file_object = open('newlvl.json', 'a')
                        file_object.write('['+omg1+']')
                        file_object.write('\n['+omg2+']')
                        file_object.write('\n['+omg3+']')
                        file_object.write('\n['+omg4+']')
                        file_object.close()
                        Menu()
                else:
                        print('Incorrect')
                        time.sleep(1)
                        Menu()
        else:
                Menu()
Menu()
