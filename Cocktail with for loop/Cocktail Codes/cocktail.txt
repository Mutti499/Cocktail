
glass_size = int(input())
straw_pos = int(input())



step = int(glass_size-(straw_pos/2)+2)
for M in range(step):

    #drawing the straw
    for x in range(straw_pos):
        for k in range(x):
            print(' ', end='')
        print('o')

    #filling the glass
    for a in range(glass_size):

        for b in range(a):
            print(' ',end='')

        print('\\',end='')

        if a+1 > M :
            for (c) in range((glass_size*2)-(a*2)):
                print('*',end='')
        else:
            for (c) in range(straw_pos-1):
                print(' ',end='')
            print('o', end='')
            for (c) in range((glass_size*2)-(a*2)-straw_pos):
                print(' ', end='')
        print('/')

    #drawing the bottom of the glass
    for b in range(glass_size):
        print(' ', end='')
    print('--')

    #drawing where you hold the glass
    for i in range(glass_size):
        for b in range(glass_size):
            print(' ', end='')
        print('||')



