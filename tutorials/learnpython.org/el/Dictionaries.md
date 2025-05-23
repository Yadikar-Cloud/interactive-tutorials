A dictionary είναι ένας τύπος δεδομένων παρόμοιος με τους πίνακες, αλλά λειτουργεί με κλειδιά και τιμές αντί με δείκτες. Κάθε τιμή αποθηκευμένη σε ένα dictionary μπορεί να προσπελαστεί χρησιμοποιώντας ένα κλειδί, το οποίο μπορεί να είναι οποιοδήποτε τύπος αντικειμένου (μια συμβολοσειρά, ένας αριθμός, μια λίστα, κτλ.) αντί να χρησιμοποιούμε το δείκτη του για την πρόσβαση.

Για παράδειγμα, μια βάση δεδομένων τηλεφωνικών αριθμών θα μπορούσε να αποθηκευτεί χρησιμοποιώντας ένα dictionary όπως αυτό:

Εναλλακτικά, ένα dictionary μπορεί να αρχικοποιηθεί με τις ίδιες τιμές χρησιμοποιώντας την παρακάτω σημειογραφία:

### Iterating over dictionaries

Τα dictionaries μπορούν να περαστούν σε επανάληψη, ακριβώς όπως μια λίστα. Ωστόσο, σε αντίθεση με μια λίστα, ένα dictionary δεν διατηρεί τη σειρά των αποθηκευμένων τιμών. Για να επαναλάβετε τα ζεύγη κλειδιού-τιμής, χρησιμοποιήστε την παρακάτω σύνταξη:

### Removing a value

Για να αφαιρέσετε ένα καθορισμένο δείκτη, χρησιμοποιήστε μία από τις παρακάτω σημειογραφίες:

ή:

Exercise
--------

Προσθέστε τον "Jake" στο phonebook με τον τηλεφωνικό αριθμό 938273443, και αφαιρέστε την Jill από το phonebook.