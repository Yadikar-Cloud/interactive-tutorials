Tutorial
--------

تىزىملىكنى چۈشىنىش ئىنتايىن كۈچلۈك قورال بولۇپ ، ئۇ باشقا تىزىملىككە ئاساسەن يېڭى تىزىملىك قۇرالايدۇ ، يەككە ، ئوقۇغىلى بولىدىغان قۇر.

مەسىلەن ، بىز ھەر بىر سۆزنىڭ ئۇزۇنلۇقىنى مەلۇم جۈملىدە بەلگىلەيدىغان پۈتۈن سانلار تىزىملىكى قۇرۇشىمىز كېرەكلىكىنى ئېيتايلى ، ئەمما بۇ سۆز «the» سۆزى بولمىسا.

    sentence = "the quick brown fox jumps over the lazy dog"
    words = sentence.split()
    word_lengths = []
    for word in words:
          if word != "the":
              word_lengths.append(len(word))
    print(words)
    print(word_lengths)

تىزىملىكنى چۈشىنىش ئارقىلىق ، بۇ ئىزاھاتقا بۇ جەرياننى ئاددىيلاشتۇرالايمىز:

    sentence = "the quick brown fox jumps over the lazy dog"
    words = sentence.split()
    word_lengths = [len(word) for word in words if word != "the"]
    print(words)
    print(word_lengths)

چېنىقىش
--------

تىزىملىكنى چۈشىنىش ئارقىلىق تىزىملىكتىن «يېڭى تىزىملىك» دەپ ئاتىلىدىغان يېڭى تىزىملىك قۇرۇڭ ، بۇ تىزىملىكتىكى ئاكتىپ سانلارنىلا ئۆز ئىچىگە ئالىدۇ.

Tutorial Code
-------------
numbers = [34.6, -203.4, 44.9, 68.3, -12.2, 44.6, 12.7]
newlist = []
print(newlist)

Expected Output
---------------

test_output_contains("[34, 44, 68, 44, 12]")
success_msg("Very nice!")

Solution
--------
numbers = [34.6, -203.4, 44.9, 68.3, -12.2, 44.6, 12.7]
newlist = [int(x) for x in numbers if x > 0]
print(newlist)
