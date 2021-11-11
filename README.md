# FP2-F02-Writing-Files
#Making a song playlist

#Ben Walz
#Writing Files FP2 FO2
#Nov 10


#funtions

def addsong():
    go = True
    
    
    playlist = open(name, 'w')
    print("What songs do you want to add? When finished, type 'done'.")
    while go == True:
        
        adding = input("> ")
        if adding == 'done' or adding == 'Done':
            go = False
        else:
            adding = adding + ', '
            playlist.write(adding)

    
    
def main():
    global name
    name = input("What do you want to name your playlist > ")
    name = name + '.txt'
    addsong()
    
    
    
#Main    
main()
    

