# reconstructSentence.py
# Jasmine Franklin
# This program accepts 2 input text files and creates a list that concatenates words while alternating from both files. 
#Usage: python3 reconstructSentence.py <file1> <file2>

import sys

def readFile(filepath):
    with open(filepath, 'r') as f:
        f_contents = f.read().split()
        f.close()
    return len(f_contents), f_contents

def writeFile(filepath, contents):
    with open(filepath, 'w') as f:
        f.write(contents)
        f.close()


def main():

    if len(sys.argv) !=3:
        sys.exit(3)

    INPUT1_FILEPATH = sys.argv[1]
    INPUT2_FILEPATH = sys.argv[2]
    OUTPUT_FILEPATH = 'output.txt'\

    print('')
    print ("Reading {} & {}:".format(INPUT1_FILEPATH, INPUT2_FILEPATH))


    #Reads each file and gets length of each file
    file1_length, f1_contents = readFile(INPUT1_FILEPATH)
    file2_length, f2_contents = readFile(INPUT2_FILEPATH)

    print('')
    print ("List 1: ")
    print (f1_contents)
    print('')
    print ("Length of List 1: {}".format(file1_length))
        

    print('')
    print ("List 2: ")
    print (f2_contents)
    print('')
    print ("Length of list 2: {}".format(file2_length))
    

    #Reconstruct Sentence
    out=[]
    while file_length > 0:
        if f1_contents:
            out.append('{} '.format(f1_contents.pop()))
        if f2_contents:
            out.append('{} '.format(f2_contents.pop()))
        file_length -= 1

    #Write string to file
    sentence = ''.join(out)

    print('')
    print("Reconstructed Sentence: ")
    print (sentence)

    writeFile(OUTPUT_FILEPATH, sentence)

    print ('')
    print ("File written to {}!".format(OUTPUT_FILEPATH))
    print('')
