Tutorial
--------
كىرگۈزۈش ۋە لازىملىق ئۇسۇلدا چىقىرىشنى كۆرسىتىش ئۆز-ئارا كودلاشتا مۇھىم رول ئوينايدۇ. شۇڭا دىققەتنى كىرگۈزۈشكە ۋە
ھەر خىل سانلىق مەلۇمات تىپلىرىنىڭ چىقىرىلىشى.

### input ()
بۇ قۇرنىڭ ئاخىرىغا بارسىلا كىرگۈزۈشكە ئىشلىتىلىدۇ. بوشلۇق بولماسلىقى كېرەكلىكىنى ئەسكەرتىڭ. كىرگۈزۈش يېڭى قۇر ھەرپ بىلەن ئاخىرلىشىدۇ ، ئەگەر كىرگۈزۈش لىنىيىسىدە بوشلۇق بولسا خاتالىق كېلىپ چىقىدۇ

    # Prints out the input received from stdin
    astring=input()# give hello as input
    print(input())

كىرگۈزۈشنى ئالغاندىن كېيىن int () ، float () ، str () قاتارلىق ئىقتىدارلارنى ئىشلىتىپ ئۇلارنى لازىملىق سانلىق مەلۇمات تىپىمىزغا ئايلاندۇرالايمىز.

    num=int(input())
    print num
    decimalnum=input()
    decimalnum=float(input()
    print decimalnum

### بوشلۇق ئارقىلىق ئايرىلغان بىر قۇردىن كىرگۈزۈش سۈپىتىدە ئىككى ياكى ئۇنىڭدىن ئارتۇق سانلىق مەلۇمات تۈرىنى قانداق ئېلىش كېرەك؟
بۇ يەردە بۆلۈش () ۋە خەرىتە () ئىقتىدارلىرىنى ئىشلىتىمىز

    #give two integers in first line and more than two integers in third line
    a, b = map(int, input().split())
    array = input().split()
    sum = 0
    for each in array:
        sum = sum + int(each)
    print(a, b, sum)  # prints first two integers from first line and sum of integers of second line

### چىقىرىش فورماتى
باسما باياناتىنىڭ ئاپتوماتىك ھالدا يېڭى قۇر قىستۇرغانلىقىنى ھېس قىلغان بولۇشىڭىز مۇمكىن. يۇقارقى كودتىكىگە ئوخشاش پەشنىڭ ئىشلىتىلىشى بوشلۇق بىلەن ئايرىلغان يەككە قۇردىكى قىممەتلەرنى بېسىپ چىقىرىدۇ.
Sys مودۇلى چىقىرىش فورماتى ئۈچۈن ھەر خىل ئىقتىدارلار بىلەن تەمىنلەيدۇ ، ئەمما بۇ يەردە فورماتلاشنىڭ ئاساسلىق بىلىملىرىنى تەلەپ بويىچە چىقىرىش ئۈچۈن ئىشلىتىشنى ئۆگىنىمىز. چىقىرىش فورماتىنى ئۆگىنىدىغان بىر قانچە مىسالنى كۆرۈپ باقايلى

    a = 5
    b = 0.63
    c = "hello"
    print("a is : %d, b is %0.4f,c is %s" % (a,b,c))

چىقىرىش چوقۇم ئۆزى چۈشەندۈرۈشى كېرەك.

چېنىقىش
--------

ئىشلەتكۈچىدىن ئۇلارنىڭ ئىسمى ، يېشى ۋە دۆلىتىنى كىرگۈزۈشىنى تەلەپ قىلىدىغان پروگرامما يېزىڭ. پروگرامما ئاندىن بۇ ئۇچۇرلارنى جۈملىگە ئۆز ئىچىگە ئالغان ئۇچۇرنى بېسىپ چىقىرىشى كېرەك. بۇ پروگرامما تۆۋەندىكىلەرنى ئۆز ئىچىگە ئېلىشى كېرەك:

1. «كىرگۈزۈش ()» ئارقىلىق ئىسىم سۈپىتىدە كىرگۈزۈش.
2. `input () using ئارقىلىق ياشنى كىرگۈزۈش ، ھەمدە ئۇنى سانغا ئايلاندۇرۇش.
3. `input () using ئارقىلىق دۆلەت نامىنى كىرگۈزۈش.
4. ئىسىم ، ياش ۋە دۆلەتنى ئۆز ئىچىگە ئالغان جۈملىنى كۆرسىتىش ئۈچۈن چىقىرىشنى فورماتلاش.

بۇ پروگرامما Python دا كىرگۈزۈش بىر تەرەپ قىلىش ۋە تىزما فورماتنى كۆرسىتىشى كېرەك.

Tutorial Code
-------------

    # Taking the name input using input()
    name = input("Enter your name: ")
    
    # Taking the age input using input() and converting it to integer
    age = int(input("Enter your age: "))
    
    # Taking the country input using input()
    country = input("Enter your country: ")
    
    # Displaying the formatted sentence with name, age, and country
    print("Hello, my name is {}, I am {} years old, and I am from {}.".format(name, age, country))


Expected Output
---------------

    Enter your name: John
    Enter your age: 25
    Enter your country: USA
    Hello, my name is John, I am 25 years old, and I am from USA.
    

Solution
-------------

    # Taking the name input using input()
    name = input("Enter your name: ")
    
    # Taking the age input using input() and converting it to integer
    age = int(input("Enter your age: "))
    
    # Taking the country input using input()
    country = input("Enter your country: ")
    
    # Displaying the formatted sentence with name, age, and country
    print("Hello, my name is {}, I am {} years old, and I am from {}.".format(name, age, country)) name is {}, I am {} years old, and I am from {}.".format(name, age, country))
