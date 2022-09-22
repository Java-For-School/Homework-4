# משימה 4:

### שאלה 5:

![alt](https://i.imgur.com/WUc7KBl.png)

##### טבלאת המעקב:
Variable | num1 | num2 | num3 | check |
--- | --- | --- | --- | --- |
Value | 6 | 45 | 73 | 0 | 
Value | 6 | 45 | 73 | 1 |
Value | 6 | 45 | 73 | 2 |

##### מטרת התוכנית:
לוודא שבין שלושה מספרים א1, א2, א3 סורר המצב הבא: א1 < א2 < א3.

### שאלה 6:
```java
import java.util.Scanner;

class HelloWorld {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        double first, second, third;
        
        first = scanner.nextDouble();
        second = scanner.nextDouble();
        third = scanner.nextDouble();
        
        if (first > second + third || second > first + third || third > first + second) System.out.println("YES");
        else System.out.println("NO");
        
    }
}
```
### שאלה 7:
```java
import java.util.Scanner;

class HelloWorld {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        int number = scanner.nextInt();
        if (number < 100 || number > 999) return;
        
        if (number % 10 == number / 10 % 10 || number % 10 == number / 100 % 10 || number / 10 % 10 == number / 100 % 10) System.out.println("Repeating");
        else System.out.println("Unique");
        
    }
}
```

### שאלה 8:
```java
import java.util.Scanner;
import java.io.IOException;

class HelloWorld {
    public static void main(String[] args) throws IOException {
        Scanner scanner = new Scanner(System.in);
        
        int number = scanner.nextInt();
        if (number < 100 || number > 999) throw new IOException("Input is invalid");
        
        int first, second, third;
        first = number % 10;
        second = number / 10 % 10;
        third = number / 100 % 10;
        if (first > 5 && second > 5 && third > 5) System.out.println("BIG");
        else if (!(first > 5 || second > 5 || third > 5)) System.out.println("SMALL");
        else System.out.println("MIXED");
        
    }
}
```

### שאלה 9:
```java
import java.util.Scanner;
import java.io.IOException;

class HelloWorld {
    public static void main(String[] args) throws IOException {
        Scanner scanner = new Scanner(System.in);
        
        int number = scanner.nextInt();
        if (number < 100 || number > 999) throw new IOException("Input is invalid");
        
        int first, second, third;
        first = number % 10;
        second = number / 10 % 10;
        third = number / 100 % 10;
        
        if ((first % 2 == 1) && (second % 2 == 1) && (third % 2 == 1)) System.out.println("ODD");
        if ((first % 2 == 0) && (second % 2 == 0) && (third % 2 == 0)) System.out.println("EVEN");
        else System.out.println("MIXED");
        
    }
}
```

![alt](https://i.imgur.com/tNVnrY6.png)
