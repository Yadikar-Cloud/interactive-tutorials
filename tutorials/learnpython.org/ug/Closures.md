Tutorial
--------

يېپىلىش فۇنكسىيە ئوبيېكتى بولۇپ ، گەرچە ئۇلار ئىچكى ساقلىغۇچتا بولمىسىمۇ ، قورشاۋ دائىرىسىدىكى قىممەتلەرنى ئەستە ساقلايدۇ. ئۇنىڭغا قەدەممۇ-قەدەم يېتىپ بارايلى

بىرىنچىدىن ، ** ئۇلانغان ئىقتىدار ** باشقا ئىقتىدارنىڭ ئىچىدە ئېنىقلانغان ئىقتىدار. دىققەت قىلىشقا تېگىشلىكى شۇكى ، ئۇلانغان ئىقتىدارلار ئۆز ئىچىگە ئالغان دائىرىنىڭ ئۆزگەرگۈچى مىقدارلىرىنى زىيارەت قىلالايدۇ. قانداقلا بولمىسۇن ، بوغما يىلاندا ئۇلار پەقەت ئوقۇشقا بولىدۇ. قانداقلا بولمىسۇن ، بۇ ئۆزگەرگۈچى مىقدارلار ئارقىلىق «يەرلىك بولمىغان» ئاچقۇچلۇق سۆزنى ئوچۇق-ئاشكارە ئىشلىتەلەيسىز.

مەسىلەن:

    def transmit_to_space(message):
        "This is the enclosing function"
        def data_transmitter():
            "The nested function"
            print(message)
    
        data_transmitter()
    
    print(transmit_to_space("Test message"))

بۇ «data_transmitter» ئىقتىدارى «ئۇچۇر» نى زىيارەت قىلالايدۇ. «يەرلىك بولمىغان» ئاچقۇچلۇق سۆزنىڭ ئىشلىتىلىشىنى كۆرسىتىش ئۈچۈن ، بۇنى ئويلاڭ

    def print_msg(number):
        def printer():
            "Here we are using the nonlocal keyword"
            nonlocal number
            number=3
            print(number)
        printer()
        print(number)
    
    print_msg(9)

يەرلىك بولمىغان ھالقىلىق سۆز بولمىسا ، چىقىرىش «3 9» بولىدۇ ، ئەمما ، ئۇنىڭ ئىشلىتىلىشى بىلەن بىز «3 3» گە ئېرىشىمىز ، يەنى «سان» ئۆزگەرگۈچى مىقدارنىڭ قىممىتى ئۆزگەرتىلىدۇ.

ھازىر ، بىز ئۇۋىغان ئىقتىدارنى چاقىرىشتىن كۆرە ، فۇنكسىيە ئوبيېكتىنى قايتۇرىمىز. (ھەتتا ئىقتىدارلارنىڭمۇ ئوبيېكت ئىكەنلىكىنى ئېسىڭىزدە تۇتۇڭ. (بۇ Python.))

    def transmit_to_space(message):
        "This is the enclosing function"
        def data_transmitter():
            "The nested function"
            print(message)
        return data_transmitter

بىز بۇ ئىقتىدارنى تۆۋەندىكىدەك دەيمىز:


      def transmit_to_space(message):
        "This is the enclosing function"
        def data_transmitter():
            "The nested function"
            print(message)
        return data_transmitter
        
  	  fun2 = transmit_to_space("Burn the Sun!")
  	  fun2()

گەرچە «transmit_to_space ()» نىڭ ئىجرا قىلىنىشى تاماملانغان بولسىمۇ ، ئۇچۇر بىر قەدەر ساقلانغان. بۇ باشقا ئەسلى ئىقتىدارلار ئاخىرلاشقاندىن كېيىنمۇ بەزى كودلارغا سانلىق مەلۇمات ئۇلىنىدىغان بۇ تېخنىكا بوغما يىلاننى تاقاش دەپ ئاتىلىدۇ

تەكلىپ: تاقاش يەرشارى ئۆزگەرگۈچى مىقدارنى ئىشلىتىشتىن ساقلىنالايدۇ ۋە مەلۇم شەكىلدىكى سانلىق مەلۇماتلارنى يوشۇرۇش بىلەن تەمىنلەيدۇ. (مەسىلەن ، بىر سىنىپتا ئۇسۇل ئاز بولسا ، ئۇنىڭ ئورنىغا تاقاشنى ئىشلىتىڭ).

شۇنداقلا ، Python دىكى بېزەكچىلەر تاقاشتىن كەڭ كۆلەمدە پايدىلىنىدۇ.

چېنىقىش
--------

ئۇۋا ھالقىسى ۋە بوغما يىلان تاقاپ ، تاقاش ئارقىلىق كۆپ كۆپەيتىش ئىقتىدارىغا ئېرىشىش ئۈچۈن ئىقتىدار قىلىڭ. يەنى تاقاشنى ئىشلىتىۋاتىدۇ ، تاقاش ئارقىلىق multiply_with_5 () ياكى multiply_with_4 () فۇنكسىيەسىنى قۇرغىلى بولىدۇ.

Tutorial Code
-------------

# your code goes here

multiplywith5 = multiplier_of(5)
multiplywith5(9)

Expected Output
---------------

test_output_contains("45")
success_msg("Great work!")

Solution
--------

def multiplier_of(n):
    def multiplier(number):
        return number*n
    return multiplier

multiplywith5 = multiplier_of(5)
print(multiplywith5(9))
