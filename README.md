# HomeWork
//დაწერეთ ფუქნცია, სახელად sayHello, რომელიც დაპრინტავს - "Hello, World".

function sayHello(){
    return "hello, world"
}
console.log(sayHello());*/


//დაწერეთ ფუნქცია, სახელად greet, რომელიც პარამეტრა მიიღებს სახელს და დაპრინტავს - "გამარჯობა, [სახელი]"
let x=prompt("შემოიყვანე სახელი");
function greet(){ 
    let y=prompt(`გამარჯობა, ${x}`)

}

greet()*/

//დაწერეთ ფუნქცია, სახელად sum, რომელიც არგუმენტებად მიიღებს ორ რიცხვს და დააბრუნებს მათ ჯამს. შედეგი გამოიტანეთ ტერმინალში.
function sum(x,y){
    return x+y;
}
console.log(sum(5,8))
*/

//დაწერეთ ფუნქცია, სახელად calculateArea, რომელიც არგუმენტად მიიღებს ოთხკუთხედის სიგრესა და სიგანეს და დააბრუნებს მის ფართობს. შედეგი გამოიტანეთ ტერმინალში.
function calculateArea(x,y){
    let c=x*y;
    return c
}
console.log(calculateArea(10,15));*/


//დაწერეთ ფუნქცია, რომელიც მიიღებს ორ არგუმენტს და დააბრუნებს მათ შორის უდიდესს. გამოიყენეთ სამივე - Function Declaration, Function Expression, Arrow Function.

function udidesi(x,y){
    if (x>y){
        return x
    }else{
        return y
    }
}
console.log(udidesi(67,90))*/

//დაწერეთ ფუქნცია, რომელიც პარამეტრად მიიღებს იმ რაოდენობას, რამდენჯერად უნდა გამოკონსოლდეს "Hello, World".

let x="hello world"
function parametri(y){
    return x.length * y;

}


//დაწერეთ პროგრამა, რომ იპოვოთ მასივის ყველა რიცხვის ჯამი.


let x=[1,2,3,4,5,6,7,8,9,10]
let y=0
for(let num of x){
    y+=num
}
    console.log(y)*/

    //დაწერეთ პროგრამა მასივში რიცხვების საშუალოს საპოვნელად.

  let numbers = [1, 2, 6, 10, 24];
let sum = 0;

function average() {
    for (let num of numbers) {
        sum += num; // ყველა რიცხვს ვუმატებთ ჯამს
    }
    let result = sum / numbers.length; // ვყოფთ ელემენტების რაოდენობაზე
    console.log("საშუალო არის:", result);
}

average();*/
//დაწერეთ პროგრამა რიცხვების მასივის ზრდის მიხედვით დასალაგებლად.

let numbers=[1,2,4,5,6,3,2,10,76,35]
numbers.sort((a,b)=>a-b)
console.log(numbers);*/

//დაწერეთ პროგრამა მასივში ყველაზე დიდი ელემენტის მოსაძებნად. ეს მარტივი გზაა
let massive=[1,2,3,4,5,6,7,8,10,23,35,64,57,68,67,100000]
let x=Math.max(...massive);
console.log(x)*/

let numbers=[1,2,4,5,6,3,2,10,76,35];
let max=numbers[0]
for(let man of numbers){
    if (man>max){
        max=man
        
    }
}
console.log(max)*/
//აწერეთ პროგრამა მასივის ყველაზე პატარა ელემენტის მოსაძებნად.
let numbers=[1,40,4,5,6,3,2,10,76,35];
let min=numbers[0]
function witchIsSmall(){
    for (let num of numbers){
        if(num<min){
            min=num
        }
    }
    console.log(min)
}
witchIsSmall();*/
//დაწერეთ პროგრამა, რათა შეამოწმოთ, შეიცავს თუ არა მასივი კონკრეტულ ელემენტს.
let numbers=[1,40,4,5,6,3,2,10,76,35];
function aahah(){
    for(let num of numbers){
        if(num===45){
            return "შეიცაvs"
        }
        
    }
    return "ara"
}
console.log(aahah())*/
//დაწერეთ პროგრამა მასივიდან ელემენტის ამოსაღებად.
let numbers=[1,40,4,5,6,3,2,10,76,35];
numbers.pop()
console.log(numbers)
numbers.shift()
console.log(numbers)
numbers.unshift(78);
console.log(numbers)
numbers.push(90);
console.log(numbers)*/

//დაწერეთ პროგრამა, რომ იპოვოთ მასივის ყველა ლუწი რიცხვის ჯამი.

 let numbers=[1,40,4,5,6,3,2,10,76,35];
 let somo=0;
 function aahah(){
    for (let sum of numbers){
        if(sum%2===0){
            somo+=sum
            
        }
    }
     console.log(somo)
 }
aahah();*/
//დაწერეთ პროგრამა მასივში სიდიდით მეორე რიცხვის მოსაძებნად.?????
let numbers=[1,40,4,5,6,3,2,10,76,35];
let max=0;
function aahah(){
    for(let num of numbers){
       let max1=Math.max(...num)
       let newMAX1=max1.spli
    }
}*/
//დაწერეთ პროგრამა რომ ორი სორტირებული მასივის შერთდეს და გახდეს ერთი მასივი რომელიც ასევე სორტირებული იქნება.
let numbers=[1,40,4,5,6,3,2,10,76,35];
let numbers2=[45,78,97,79,3522,2413]
numbers.sort((a,b)=>a-b);
numbers2.sort((a,b)=>a-b);
let saerto=[...numbers,...numbers2].sort((a,b)=>a-b);
console.log(saerto)*/
//დაწერეთ პროგრამა სტრიქონების მასივის ანბანის მიხედვით დასალაგებლად.\
let fruits = ["banana", "apple", "cherry", "mango", "kiwi"];
fruits.sort();
console.log(fruits);*/
//შექმენით ობიექტი სახელწოდებით car თვისებებით მარკის, მოდელისა და წლისთვის. დაბეჭდეთ ობიექტი კონსოლზე.
let car={
        mark:"bmw",
        model:"c450",
        year:"2005",
        start:function(){
            console.log("The car is starting!")
        }
}
//დაამატეთ მეთოდი car ობიექტს სახელწოდებით start, რომელიც ბეჭდავს "The car is starting!" როდესაც გამოძახება. გამოიძახეთ დაწყების მეთოდი.
car.start();*/
//შექმენით სხვა ობიექტი სახელად Person სახელის, ასაკისა და ქალაქის თვისებებით. დაბეჭდეთ სახელის თვისება წერტილის გამოყენებით.
let Person={
        age:23,
        city:"tbilisi",
        name:"temo"

}
console.log(Person.name)

//დაამატეთ ახალი თვისება სახელწოდებით job, Person ობიექტს და მიანიჭეთ მას მნიშვნელობა. დაბეჭდეთ განახლებული ობიექტი.

Person.job="araferi";
console.log(Person);
//პროექტი 10 - ქულების გამომთვლელი
//შექმენით მარტივი JavaScript პროგრამა, რომელიც ითვლის შეფასებას მოსწავლის ქულების მიხედვით.
//შეფასების სქემა შემდეგნაირია:
//A: 90-100
//B: 80-89
//C: 70-79
//D: 60-69
//F: 0-59
//პროგრამამ უნდა მოსთხოვოს მომხმარებელს შეიყვანოს რიცხვითი ქულა(0-დან 100-ის ჩათვლით ნებისმიერი რიცხვი).
//გამოიყენეთ პირობითი ოპერატორები შეყვანილი რიცხვის შეფასების დასადგენად.
//ეკრანზე გამოიტანეთ როგორც შეყვანილი რიცხვი ასევე შესაბამისი ასო.

//
function check() {
    let question = Number(prompt("შემოიყვანეთ თქვენი ქულა (0-100):"));
    
    
    while (isNaN(question) || question < 0 || question > 100) {
        question = Number(prompt("შეიყვანეთ მხოლოდ რიცხვი 0-დან 100-მდე!"));
    }

    return question; 
}

function result() {
    let question = check();

    if (question >= 90) {
        return `A: ${question}`;
    } else if (question >= 80) {
        return `B: ${question}`;
    } else if (question >= 70) {
        return `C: ${question}`;
    } else if (question >= 60) {
        return `D: ${question}`;
    } else {
        return `F: ${question}`;
    }
}

console.log(result());*/

//პროექტი 10 - ქულების გამომთვლელი,
/*Simple Math - მარტივი მათემატიკა,
თქვენ ხშირად დაწერთ პროგრამებს, რომლებიც ეხება რიცხვებს. ხშირად, პროგრამაში მიღებული მონაცემები (input )რიცხვით მონაცემების ტიპებად უნდა გარდაქმნათ. 
დაწერეთ პროგრამა, რომელიც მოგთხოვთ ორ რიცხვს. ამობეჭდეთ ამ რიცხვების ჯამი, სხვაობა, ნამრავლი და განაყოფი.

მაგალითად:
> What is the first number? 10
> What is the second number? 5
> 10 + 5 = 15
> 10 - 5 = 5
> 10 * 5 = 50
> 10 / 5 = 2
*/
function check() {
  let firstNumber = Number(prompt("What is the first number?"));
  let secondNumber = Number(prompt("What is the second number?"));

  while (isNaN(firstNumber) || isNaN(secondNumber)) {
    alert("Enter only numbers!");
    firstNumber = Number(prompt("What is the first number?"));
    secondNumber = Number(prompt("What is the second number?"));
  }

  // ვაბრუნებთ ობიექტად ორივე რიცხვს
  return { firstNumber, secondNumber };
}

function calculateArea() {
  let numbers = check(); // ვიღებთ ობიექტს { firstNumber, secondNumber }
  let a = numbers.firstNumber;
  let b = numbers.secondNumber;

  let sum = a + b;
  let difference = a - b;
  let product = a * b;
  let division = a / b;

  console.log("Sum:", sum);
  console.log("Difference:", difference);
  console.log("Product:", product);
  console.log("Division:", division);
}

calculateArea();
