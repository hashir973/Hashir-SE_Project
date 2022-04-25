import 'dart.io';

void main() {
   print("Enter First Number");
   var fn = int.parse(stdin.readLineSync()!);
   print("Enter Second Number");
   var sn = int.parse(stdin.readLineSync()!);
   print("Operation to be performed from +,-,*,/");
   var op = stdin.readLineSync();
     if (op == '+') {
        var result = fn + sn;
        print('The Sum of your given numbers are $result');
   }
   if (op == '-') {
       var result = fn - sn;
       print('The Subtraction of your given numbers are $result');
   }
   if (op == '*') {
       num result = fn * sn;
       print('The Multiplication of your given numbers are $result');
   }
   if (op == '/') {
       num result = fn ~/ sn;
       print('The Division of your given numbers are $result');
   }
   if (op != '+' && op != '-' && op != '*' && op != '/') {
       print('Invalid Operation Given');
   }
 }
