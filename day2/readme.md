```c#
using System;

class Program {
  public static void Main (string[] args) {
    string [] test = System.IO.File.ReadAllLines(@"Input.txt");
    int score = 0;
    foreach(string i in test){
      if(i[0] == 'A'){
        if(i[2] == 'Y'){
          score+=4;
        }
        else if(i[2] == 'X'){
          score+=3;
        }
        else if(i[2] == 'Z'){
          score+=8;
        }
      }
      else if(i[0] == 'B'){
        if(i[2] == 'Y'){
          score+=5;
        }
        else if(i[2] == 'X'){
          score+=1;
        }
        else if(i[2] == 'Z'){
          score+=9;
        }
      }
      else if(i[0] == 'C'){
        if(i[2] == 'Y'){
          score+=6;
        }
        else if(i[2] == 'X'){
          score+=2;
        }
        else if(i[2] == 'Z'){
          score+=7;
        }
      }
    }
      Console.WriteLine(score);
  }
}
```
