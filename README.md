<div align="center">

## Precise Calculation of Pi


</div>

### Description

This code calculates an estimated value of Pi using the Leibnitz series (which is basically a power series expansion of a trigonometric function which allows to estimate Pi very well)
 
### More Info
 
Prints the estimated value of Pi


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Eli](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/eli.md)
**Level**          |Beginner
**User Rating**    |4.8 (19 globes from 4 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/eli-precise-calculation-of-pi__3-360/archive/master.zip)

### API Declarations

```
iostream.h
math.h
```


### Source Code

```
#include <iostream.h>
#include <math.h>
#define NUM_OF_ELEMENTS 20000
int main()
{
 double pi = 0;
 // Calculating pi/4
 for (long int n = 1; n <= NUM_OF_ELEMENTS; n++)
 {
 pi += (double) pow(-1, n+1)/(2*n-1);
 }
 // Calculating pi
 pi *= 4;
 cout << "Estimated PI value (" << NUM_OF_ELEMENTS << " elements of Leibnitz series): "<< pi;
 return 0;
}
```

