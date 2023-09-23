# Bacagine

I'm a 6th semester student studying Systems Analysis and Development at FATEC.

C/C++ Developer.

Linux User (Arch Linux)

See bellow a brief explanation of the coding method I use in my programs

## Hungarian Notation
In my programs I use a customized version of Hungarian Notation.

Hungarian notationaims to facilitate recognition of the type of variable in a program, just by looking at the name of the variable.
See below a table with the type of indicators for each type of data.

| Indicator    | Type         |
| :---------:  | :-------:    |
| g            | Global       |
| k            | Constant     |
| a            | Array        | 
| p            | Pointer      |
| v            | Void         |
| b            | Boolean      |
| c            | Char         |
| i            | Integer      |
| f            | Float        |
| d            | Double       |
| sz           | String       |
| st           | Structure    |
| u            | Union        |
| e            | Enum         |
| fp           | File Pointer |

### Hungarian Notation Usage Example
```c

typedef struct Person
{
  int iID;
  char szName[64];
  char cSex;
  float fHeight;
  double dSalary;
  bool bLive;
} Person, *PPerson

const double gkdPI = 3.14; 

...

int main(int argc, char **argv)
{
  Person * pstPerson = (PPerson) malloc(sizeof(Person);
  
  ...
  
  free(pstPerson);
  pstPerson = NULL;
  
  return 0;
}

```

