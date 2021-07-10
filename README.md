# cpp_notes
## extern
extern int i; // just declare i

int j; // declare and define j

file1.hpp
```
int j = 3;
```

file2.cpp
```#include "file1.hpp"
#include <iostream>
extern int j;
int main() {
    using namespace std;
    cout << j << endl;
}
```
  
`output: 3`
  
## reference
referency type provides an alias for another type
  
```
#include<iostream>

int main(){
    using namespace std;
    int i = 888;
    int &refVal = i;
    refVal = 999;
    cout << "i = " << i << endl;
}

```
output: 999
  
refVal points the value referenced by i, so changes made to refVal directly reflected by i

## void *
void * is a generic pointer which can points to any type of pointer
