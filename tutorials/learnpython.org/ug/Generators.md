Tutorial
--------

گېنېراتورلارنى يولغا قويۇش ناھايىتى ئاسان ، ئەمما چۈشىنىش بىر ئاز قىيىن.

گېنېراتورلار تەكرارلىغۇچ ياساشقا ئىشلىتىلىدۇ ، ئەمما باشقىچە ئۇسۇل بىلەن. گېنېراتورلار ئاددىي ئىقتىدارلار بولۇپ ، تەكرارلىنىدىغان بىر يۈرۈش تۈرلەرنى بىر-بىرلەپ ئالاھىدە ئۇسۇلدا قايتۇرىدۇ.

بىر يۈرۈش تۈر ئۈستىدىكى تەكرارلىنىش باياننى ئىشلىتىشكە باشلىغاندا ، گېنېراتور ئىجرا بولىدۇ. گېنېراتورنىڭ ئىقتىدار كودى «ھوسۇل» باياناتىغا يەتكەندىن كېيىن ، گېنېراتور ئىجرا قىلىنىشىنى قايتىدىن دەۋرىيلىككە قايتۇرىدۇ ، يۈرۈشلۈكتىن يېڭى قىممەت قايتۇرىدۇ. گېنېراتور ئىقتىدارى ئۆزى خالىغانچە قىممەت ھاسىل قىلالايدۇ (چەكسىز بولۇشى مۇمكىن) ، ھەر بىرسىنى ئۆز نۆۋىتىدە بېرىدۇ.

بۇ يەردە 7 ئىختىيارى پۈتۈن ساننى قايتۇرىدىغان گېنېراتور ئىقتىدارىنىڭ ئاددىي بىر مىسالى بار:

      import random
      
      def lottery():
          # returns 6 numbers between 1 and 40
          for i in range(6):
              yield random.randint(1, 40)
      
          # returns a 7th number between 1 and 15
          yield random.randint(1, 15)
      
      for random_number in lottery():
             print("And the next number is... %d!" %(random_number))

بۇ ئىقتىدار تاسادىپىي سانلارنى قانداق قىلىپ ئۆزلۈكىدىن ھاسىل قىلىشنى قارار قىلىدۇ ھەمدە مەھسۇلات باياناتىنى بىر-بىرلەپ ئىجرا قىلىدۇ ، ئارىلىقتا توختاپ نەتىجىنى ئاساسىي ھالقا ئايلاندۇرىدۇ.

چېنىقىش
--------

Fibonacci يۈرۈشلۈكىنى قايتۇرىدىغان گېنېراتور ئىقتىدارىنى يېزىڭ. ئۇلار تۆۋەندىكى فورمۇلا ئارقىلىق ھېسابلىنىدۇ: يۈرۈشلۈك ئالدىنقى ئىككى سان ھەمىشە 1 گە تەڭ ، ئۇدا قايتۇرۇلغان ھەر بىر سان ئاخىرقى ئىككى ساننىڭ يىغىندىسى.
ئەسكەرتىش: گېنېراتور ئىقتىدارىدا پەقەت ئىككى ئۆزگەرگۈچى مىقدارنى ئىشلىتەمسىز؟ تاپشۇرۇقنى بىرلا ۋاقىتتا قىلغىلى بولىدىغانلىقىنى ئېسىڭىزدە تۇتۇڭ. كود

    a = 1
    b = 2
    a, b = b, a
    print(a, b)

بىرلا ۋاقىتتا a ۋە b نىڭ قىممىتىنى ئالماشتۇرىدۇ.

Tutorial Code
-------------

# fill in this function
def fib():
    pass #this is a null statement which does nothing when executed, useful as a placeholder.

# testing code
import types
if type(fib()) == types.GeneratorType:
    print("Good, The fib function is a generator.")

    counter = 0
    for n in fib():
        print(n)
        counter += 1
        if counter == 10:
            break



Expected Output
---------------

test_output_contains("Good, The fib function is a generator.")
success_msg('Good work!')

Solution
--------

# fill in this function
def fib():
    a, b = 1, 1
    while 1:
        yield a
        a, b = b, a + b

# testing code
import types
if type(fib()) == types.GeneratorType:
    print("Good, The fib function is a generator.")

    counter = 0
    for n in fib():
        print(n)
        counter += 1
        if counter == 10:
            break
