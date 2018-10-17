safe_numerics
=============

Arithmetic operations in C++ are NOT guaranteed to yield a correct mathematical result. This feature is inherited from the early days of C. The behavior of int, unsigned int and others were designed to map closely to the underlying hardware. Computer hardware implements these types as a fixed number of bits. When the result of arithmetic operations exceeds this number of bits, the result is undefined and usually not what the programmer intended. It is incumbent upon the C++ programmer to guarantee that this behavior does not result in incorrect behavior of the program. This library implements special versions of these data types which behave exactly like the original ones EXCEPT that the results of these operations are checked to be sure that an exception will be thrown anytime an attempt is made to store the result of an undefined operation.

Note: This is the subject of a recent presentation at CPPCon 2017.  https://www.youtube.com/watch?v=93Cjg42bGEw .
