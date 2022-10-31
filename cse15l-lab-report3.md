1. grep -i [string] [file name]

- this command-line option, -i, displays the line that contains [string] in the file, regardless of lower or upper case.

minsangkim@Min-Kims-MBP path-examples % grep -i "import" Read.java
import java.util.Scanner;

minsangkim@Min-Kims-MBP path-examples % grep -i "nest" some-files/even-more-files/a.txt
nested file
NESTED file
NESting

minsangkim@Min-Kims-MBP path-examples % grep -i "a" some-files/a.txt
minsangkim@Min-Kims-MBP path-examples % grep -i "h" some-files/a.txt
hello

2. grep -v [string] [file name]

- it used to display the lines which do not match with the given string.

minsangkim@Min-Kims-MBP path-examples % grep -v "import" Read.java

class Read {
public static void main(String[] args) {
System.out.print("What's your name? ");
Scanner in;
in = new Scanner(System.in);
String s = in.nextLine();
System.out.println("Hello " + s);
}
}

minsangkim@Min-Kims-MBP path-examples % grep -v "c" some-files/a.txt
hello

minsangkim@Min-Kims-MBP path-examples % grep -v "h" some-files/more-files/b.txt
i don't know
gege

3. grep -c [string] [file name]

- it counts the number of lines that contain the given string

minsangkim@Min-Kims-MBP path-examples % grep -c "a" Read.java
6

minsangkim@Min-Kims-MBP path-examples % grep -c "}" Read.java
2

minsangkim@Min-Kims-MBP path-examples % grep -c "h" some-files/even-more-files/a.txt
1
