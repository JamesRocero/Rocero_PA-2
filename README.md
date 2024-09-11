Normalization Problem
``` python
#start

#import numerical python library
import numpy as np

#create random 5 by 5 array
X = np.random.rand(5,5)

#formula for the normalized values
Z = (X - X.mean()) / X.std()

#store the normalized values in the file X_normalized.npy
np.save("X_normalized.npy",Z)

#print the original and normalized value
print ("Origial Value: \n", X, "\n Normalized Value: \n", Z)
Origial Value: 
 [[0.37821599 0.04187895 0.07844642 0.24557588 0.55283743]
 [0.74999649 0.49806591 0.75614145 0.28815916 0.3094089 ]
 [0.9281654  0.08364805 0.47308614 0.4186179  0.68921463]
 [0.64802812 0.740649   0.16926131 0.11575902 0.91036623]
 [0.99416337 0.84031066 0.45744658 0.26382506 0.49592852]] 
 Normalized Value: 
 [[-0.3781913  -1.56839919 -1.43899659 -0.8475696   0.23974782]
 [ 0.93744162  0.04592586  0.95918699 -0.69687864 -0.62168142]
 [ 1.56793428 -1.42058938 -0.04247091 -0.23521963  0.72235066]
 [ 0.57660251  0.90436329 -1.11762668 -1.30695714  1.50494771]
 [ 1.80148366  1.25703959 -0.09781518 -0.78299056  0.03836222]]

#start

#import numerical python
import numpy as np

#create array of all first 100 positive integers
A = np.array(np.arange(1,101,1))

#resize the array to be 10 rows and 10 columns
A.resize(10,10)

#holds an array that has each element squared
Squared_A = np.square(A)

#stores every element from squared_a that is divisible by 3
Divide_by_3 = Squared_A[A%3==0]

#store the array of elements that are divisible by three in 'Divide_by_3.npy'
np.save('Divide_by_3.npy',Divide_by_3)

#print the value of a
print (A)
[[  1   2   3   4   5   6   7   8   9  10]
 [ 11  12  13  14  15  16  17  18  19  20]
 [ 21  22  23  24  25  26  27  28  29  30]
 [ 31  32  33  34  35  36  37  38  39  40]
 [ 41  42  43  44  45  46  47  48  49  50]
 [ 51  52  53  54  55  56  57  58  59  60]
 [ 61  62  63  64  65  66  67  68  69  70]
 [ 71  72  73  74  75  76  77  78  79  80]
 [ 81  82  83  84  85  86  87  88  89  90]
 [ 91  92  93  94  95  96  97  98  99 100]]
 ```
