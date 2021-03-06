# Tiny C utils
Utils for C     
Define `TINY_UTILS_IMPLEMENTATION` in a file where you want the function bodys to be copied.    

`char* utils_strin()`   
Reads input without skipping space and stops if `EOF` or `\n` are passed, grows the buffer in 16 char chunks if needed, return a pointer to memory in heap, free after using it.   

`int utils_variance(int arr[], int n)`    
Returns variance of an int array.    

`int utils_frequent(int arr[], int n)`    
Returns most frequent item in an array.     

`bool* utils_sieve_prime(uint64_t n)`     
Prime sieve algorithm, returns an array on heap, index of the array indicates the number is prime or not, free after using it.     

`bool utils_is_prime(uint64_t n)`     
Checks number is prime or not, an O(sqrt(n)) is used.     

`wchar_t* utils_wstrin();`         
Wide character version of `utils_strin`.    
Define `TINY_UTILS_UNICODE` before using.      
Warning: Only tested for English, Arabic scripts.    

`utils_bit_is_set(x, n)`    
`utils_bit_set(x, n)`    
`utils_bit_reset(x, n)`     
`utils_bit_toggle(x, n)`      

Bit bit manipulation **macros**, **they do not modify the original value of `x`**, the `n` argument specifies the bit to get manipulated, the `x` arguments specifies the data.   
