
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

    // Console.Write("enter the string : ");
    // string name=Console.ReadLine();
    // string name_af="";
    // for(int i=0;i<name.Length;i++){
    //     if(name[i]=='a'){
    //         name_af=name_af+name[i]+"0";
    //     }else{
    //         name_af=name_af+name[i];
    //     }
    // }
    // Console.WriteLine($"string after add 0 after char 'a' ==> {name_af}");
    
    
    // 6 count of non_literals
    // var name="Zeh257";
    // // a-z
    // // 97-122
    // // A Z 
    // // 65  90

    // int count=0;
    // for(int i=0;i<name.Length;i++){
    //     int w=name[i];
    //   if(!((w>=97 &&w<=122)||(w>=65 && w<=90))){
    //       count++; 
    //   }
    // }
    // Console.WriteLine($"num of non_literals ==>{count} ");
    // 7) is palindrome
    // Console.Write("enter the string : ");
    // string name=Console.ReadLine();
    // // abccbw
    // // i  arr.length-1-i
    // // 0 5  6-1-0=5
    // // 1 4  6-1-1=4
    // // 2 3  6-1-2=3
    // bool pali=true;
    // for(int i=0;i<name.Length/2;i++){
    //     if(name[i]!=name[name.Length-1-i]){
    //         pali=false;
    //         break;
    //     }
    // }
    // if(pali==true){
    //     Console.WriteLine("the string is palindrome");
    // }else{
    //   Console.WriteLine("the string is not palindrome"); 
    // }
    
    // 8 remove duplicate
//     Console.Write("enter the text : ");
//   string text=Console.ReadLine();
//   string re_text="";
// //   amera
//   for(int i=0;i<text.Length;i++){
//       if(!re_text.Contains(text[i])){
//           re_text=re_text+text[i];
//       }
//   }
//   Console.WriteLine($"text without duplicate {re_text}");
    
    
    
    // 9) earliest nearest value from mean
    // var arr=new int[5]{2,4,10,8,1};
    // int sum=0;
    // for(int i=0;i<arr.Length;i++){
    //     sum=sum+arr[i];
    // }
    // float mean=sum/5;
    // Array.Sort(arr);
    // for(int i=0;i<arr.Length;i++){
    //     if(arr[i]>=mean){
    //         Console.WriteLine($" earliest nearest value from mean {arr[i]}");
    //         break;
    //     }
    // }
    // 10)  mean of the max-min values
    // Console.Write("enter the length of array : ");
    // int leng=int.Parse(Console.ReadLine());
    // var arr=new int[leng];
    // for(int i=0;i<leng;i++)
    //     arr[i]=int.Parse(Console.ReadLine());
    // int max=arr[0];
    // int min=arr[0];
    // for(int i=0;i<leng;i++){
    //     if(arr[i]>max) max=arr[i];
    //     if(arr[i]<min) min=arr[i];
    // }
    
    // float mean=(max+min)/2;
    
    // Console.WriteLine($"mean of the {max } {min} values ==> {mean} ");
    
    // 11)  missing integer
    // 4 2 4 6 7==>1
    // 5 9 10 12 
    // 1 2 3 4  =>5
    // 1 3 4 5  ==>2
    // Console.Write("enter the length of array : ");
    // int leng=int.Parse(Console.ReadLine());
    // var arr=new int[leng];
    // for(int i=0;i<leng;i++)
    //     arr[i]=int.Parse(Console.ReadLine());
    // Array.Sort(arr);
    // if(arr[0]!=1){
    //     Console.WriteLine("1");
    // }else{
    //     bool missing=false;
    //     int i=1;
    //     for(i=0;i<leng-1;i++){
    //         if(!(arr[i]==arr[i+1]-1)){
    //             missing=true;
    //             break;
    //         }
    //     }
    //     if(missing==true){
    //         Console.WriteLine(arr[i]+1);
    //     }else{
    //         Console.WriteLine(arr[i]+1);
    //     }
    // }
    // 12) num of item less than average
    // var arr=new int[5]{4,3,2,1,5};
    // float avg;
    // int sum=0;
    // for(int i=0;i<arr.Length;i++){
    //     sum=sum+arr[i];
    // }
    // avg=sum/arr.Length;
    // // Array.Sort(arr);
    // int count=0;
    // for(int i=0;i<arr.Length;i++){
    //     if(arr[i]<=avg){
    //         count++;
    //     }
    // }
    // Console.WriteLine($"num of item less than average {avg} ==> {count} ");
    
    // // 13) the fisrt larget element greater than avg
    //  var arr=new int[5]{4,3,2,1,5};
    // float avg;
    // int sum=0;
    // for(int i=0;i<arr.Length;i++){
    //     sum=sum+arr[i];
    // }
    // avg=sum/arr.Length;
    // Array.Sort(arr);
    // int max=arr[0];
    // for(int i=0;i<arr.Length;i++){
    //     if(arr[i]>avg){
    //         max=arr[i];
    //         break;
    //     }
    // }
    // Console.WriteLine($"the fisrt larget element greater than avg {avg} ==>{max} ");
    
}}
