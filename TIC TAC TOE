# TIC-TAC-TOE
def sum(a, b, c ):
    return a + b + c
    
def printBoard (xState, zState):
    zero = 'X' if xState[0] else ('Y' if zState[0] else 0)
    one = 'X' if xState[1] else ('Y' if zState[1] else 1)
    two = 'X' if xState [2] else ('Y' if zState[2] else 2)
    three= 'X' if xState[3] else ('Y' if zState[3] else 3)
    Four ='X' if xState[4] else ('Y' if zState[4] else 4)
    five = 'X' if xState[5] else ('Y' if zState[5] else 5)
    six = 'X' if xState[6] else ('Y' if zState[6] else 6)
    seven = 'X' if xState[7] else ('Y' if zState[7] else 7)
    eight='X' if xState[8] else ('Y' if zState [8] else 8)
    print(f"{zero} | {one} | {two} ")
    print(f"--|---|---")
    print(f"{three} | {Four} | {five} ")
    print(f"--|---|---")
    print(f"{six} | {seven} | {eight} ")


def checkWin(xState, zState):
    wins = [[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]]
    for win in wins:
        if(sum(xState[win[0]], xState[win[1]], xState[win[2]]) == 3):
            print("x won the match")
            return 1
        if(sum(zState[win[0]], zState[win[1]], zState[win[2]]) == 3):
            print("y Won the match")
            return 0
    return -1
    
if _name_ == "_main_":
    xState = [0, 0, 0, 0, 0, 0, 0, 0, 0] 
    zState = [0, 0, 0, 0, 0, 0, 0, 0, 0]
    turn= 1 # 1 for x and 0 for o
    print("Welcome to Tic Tac Toe")
    while(True):
        printBoard(xState, zState)
        if (turn == 1):
            print("X's Chance")
            value = int(input("Please enter a value: "))
            xState[value] = 1
        else:
            print("Y's Chance")
            value = int(input("Please enter a value: "))
            zState[value] = 1
        cwin = checkWin(xState, zState)
        if(cwin != -1):
            print("Match over")
            break
        turn = 1 - turn
