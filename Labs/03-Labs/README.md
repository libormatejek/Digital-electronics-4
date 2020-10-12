## Preperation task
Fill in the following table and enter the number of bits and numeric range for the selected data types defined by C.


|  Data type  | Number of bits |    Range      |      Description               |
|-------------|----------------|---------------|--------------------------------|
|   uint8_t   |       8        |   0,1,...255  |Unsigned 8-bit integer          |
|   int8_t    |       8        |   -128..127   |Signed 8-bit integer            |
|   uint16_t  |      16        |   0..65.535   |Unsigned 16-bit integer         |
|   int16_t   |      16        |-32,768..32767 |Signed 16-bit integer           |
|   float     |      32        |-3.4E38..3.4E38|Single-precision floating-point |
|   void      |    no data     |     no data   |no data                         |

```ruby
#include <avr/io.h>

// Function declaration (prototype)
uint16_t calculate(uint8_t, uint8_t);

int main(void)
{
    uint8_t a = 156;
    uint8_t b = 14;
    uint16_t c;

    // Function call
    c = calculate(a, b);

    return 0;
}

// Function definition (body)
 uint16_t calculate(uint8_t x, uint8_t y)
{
    uint16_t result;    // result = x^2 + 2xy + y^2

result = (x*x);
        (2*x*y);
         (y*y);
    
    return result;
}
```
