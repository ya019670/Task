using System;

public class HelloWorld
{
    public static void Main()
    {
       1)  // reverse a string
         Console.Write("enter the string : ");
       string name=Console.ReadLine();
       string reverse="";
       for(int i=name.Length-1;i>=0;i--){
           reverse=reverse+name[i];
       }
       Console.Write($"reverse string is :{reverse} ");
     }

    // 2 count of a's

       Console.Write("enter the string : ");
       string name=Console.ReadLine();
     int count=0;
     for(int i=0;i<name.Length;i++){
         if(name[i]=='a'){
             count++;
         }
     }
     Console.WriteLine($"num of a in string ==> {count}");
    
    // 3 ) last index of "a"

     Console.Write("enter the string : ");
     string name=Console.ReadLine();
     int index=0;
     for(int i=name.Length-1;i>=0;i--){
         if(name[i]=='a'){
             index=i;
             break;
         }
     }
     Console.WriteLine($"last index of 'a' ==> {index}");
    
    // 4 remove all 'a'

     Console.Write("enter the string : ");
     string name=Console.ReadLine();
     string name_af="";
     for(int i=0;i<name.Length;i++){
         if(name[i]!='a'){
             name_af=name_af+name[i];
         }
     }
     Console.WriteLine($"string after remove all 'a' ==> {name_af}");

    //  5) add 0 after each a

     Console.Write("enter the string : ");
     string name=Console.ReadLine();
     string name_af="";
     for(int i=0;i<name.Length;i++){
         if(name[i]=='a'){
             name_af=name_af+name[i]+"0";
         }else{
             name_af=name_af+name[i];
         }
     }
     Console.WriteLine($"string after add 0 after char 'a' ==> {name_af}");
       
    // 6 count of non_literals

     var name="Zeh257";
     int count=0;
     for(int i=0;i<name.Length;i++){
         int w=name[i];
       if(!((w>=97 &&w<=122)||(w>=65 && w<=90))){
           count++; 
       }
     }
     Console.WriteLine($"num of non_literals ==>{count} ");
   
    // 7) is palindrome

    Console.Write("enter the string : ");
    string name=Console.ReadLine();
     bool pali=true;
     for(int i=0;i<name.Length/2;i++){
         if(name[i]!=name[name.Length-1-i]){
             pali=false;
             break;
         }
     }
     if(pali==true){
         Console.WriteLine("the string is palindrome");
     }else{
       Console.WriteLine("the string is not palindrome"); 
     }
    
    // 8 remove duplicate

     Console.Write("enter the text : ");
   string text=Console.ReadLine();
   string re_text="";
   for(int i=0;i<text.Length;i++){
       if(!re_text.Contains(text[i])){
           re_text=re_text+text[i];
       }
   }
   Console.WriteLine($"text without duplicate {re_text}");
    
    
    // 9) earliest nearest value from mean

     var arr=new int[5]{2,4,10,8,1};
     int sum=0;
     for(int i=0;i<arr.Length;i++){
         sum=sum+arr[i];
     }
     float mean=sum/5;
     Array.Sort(arr);
     for(int i=0;i<arr.Length;i++){
         if(arr[i]>=mean){
             Console.WriteLine($" earliest nearest value from mean {arr[i]}");
             break;
         }
     }

    // 10)  mean of the max-min values

     Console.Write("enter the length of array : ");
     int leng=int.Parse(Console.ReadLine());
     var arr=new int[leng];
     for(int i=0;i<leng;i++)
         arr[i]=int.Parse(Console.ReadLine());
     int max=arr[0];
     int min=arr[0];
     for(int i=0;i<leng;i++){
         if(arr[i]>max) max=arr[i];
         if(arr[i]<min) min=arr[i];
     }
     float mean=(max+min)/2;
     Console.WriteLine($"mean of the {max } {min} values ==> {mean} ");
    
    // 11)  missing integer

     Console.Write("enter the length of array : ");
     int leng=int.Parse(Console.ReadLine());
     var arr=new int[leng];
     for(int i=0;i<leng;i++)
         arr[i]=int.Parse(Console.ReadLine());
     Array.Sort(arr);
     if(arr[0]!=1){
         Console.WriteLine("1");
     }else{
         bool missing=false;
         int i=1;
         for(i=0;i<leng-1;i++){
             if(!(arr[i]==arr[i+1]-1)){
                 missing=true;
                 break;
             }
         }
         if(missing==true){
             Console.WriteLine(arr[i]+1);
         }else{
             Console.WriteLine(arr[i]+1);
         }
     }

     //  12) num of item less than average

     var arr=new int[5]{4,3,2,1,5};
     float avg;
     int sum=0;
     for(int i=0;i<arr.Length;i++){
         sum=sum+arr[i];
     }
     avg=sum/arr.Length;
    
     Array.Sort(arr);
     int count=0;
     for(int i=0;i<arr.Length;i++){
         if(arr[i]<=avg){
             count++;
         }
     }
     Console.WriteLine($"num of item less than average {avg} ==> {count} ");
    
     // 13) the fisrt larget element greater than avg

      var arr=new int[5]{4,3,2,1,5};
     float avg;
     int sum=0;
     for(int i=0;i<arr.Length;i++){
         sum=sum+arr[i];
     }
     avg=sum/arr.Length;
     Array.Sort(arr);
     int max=arr[0];
     for(int i=0;i<arr.Length;i++){
         if(arr[i]>avg){
             max=arr[i];
             break;
         }
     }
     Console.WriteLine($"the fisrt larget element greater than avg {avg} ==>{max} ");
    
}}






//Square of a number 1
    Console.Write("Enter number to get its square");
    int x =Convert.ToInt32( Console.ReadLine());
    Console.WriteLine(x*x);


    // Average of two integers 2
    Console.Write("Enter number x1 : ");
    int x1 = Convert.ToInt32( Console.ReadLine());
    Console.Write("Enter number x2 : ");
    int x2 = Convert.ToInt32( Console.ReadLine());
    int avg = (x1 + x2)/2;
    Console.WriteLine(avg);

    // Adding N integers 3
    Console.Write("Enter number to add");
    int sizee = Convert.ToInt32(Console.ReadLine());
    int sum=0;
    for(int i=0; i<sizee; i++){
        int m =Convert.ToInt32(Console.ReadLine());
        sum+=m;
    }Console.WriteLine(sum);


    //Converting Celsius to Fahrenheit 4
    double Celsius = Convert.ToDouble(Console.ReadLine());
    double fahrenhait =(Celsius*9)/5 + 32;
    Console.WriteLine(fahrenhait);


    //Converting String to Uppercase 5
    Console.Write("Enter String To convert it to upper case : ");
    string a =Console.ReadLine();
    string converted = a.ToUpper();
    Console.WriteLine(converted);

//Max Number 7
   Console.Write("Enter number of numbers to check max");
   int size = Convert.ToInt32(Console.ReadLine());
   var arr = new int [size];
   for (int i = 0 ; i < size ; i++){
    arr[i] = Convert.ToInt32(Console.ReadLine());
    }
     int max = 0;
    for (int i = 0; i < arr.Length; i++){
       if(max < arr[i]){
        max=arr[i];
       }
    } Console.WriteLine(max);
   

   //Last Even Number 8
   Console.Write("Enter size of numbers to get Last Even Number");
    int S =Convert.ToInt32(Console.ReadLine());
     int even=0;
    for(int i=0 ; i<S; i++){
        int n=Convert.ToInt32(Console.ReadLine());
        if(n%2==0){
           even=n;
        }
    }Console.WriteLine(even);
