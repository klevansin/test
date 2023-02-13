# Команды git

0. git clone ADDR PATH - клонировать проект с github 
   ADDR - адрес прокета
   PATH - папка на компьютере куда скопируется проект

1. git pull origin main  - скачать с github
... изменили проект
2. git add . -  индексируем (предварительно сохраняем)
3. git commit -m "краткий комментарий"  - коммит, конечная фиксация
4. git push origin main - отправка кода на github
5. git status - посмотреть текущий статус проекта

# Переменные
```let <NAME> [= <VALUE>];```

пример: 
```js        
let a = 10;
let b;
```
 
 # Типы переменных
```js
let a1 = 10;            // число
let a2 = '10';          // строка
let a3 = "kaewjhfewkj"; 
// мультистрока
let a4 = `qwkejfew
welkfewrf
werferwfj
werferwf`;
let a5 = true;          // bool
let a6 = false;
let a7 = null;          // null
let a8 = undefined;     // не определено
```

# Сравнение

```js
let r; // let r = undefined;
let kk = undefined;

if (kk == r){ // kk = null; kk = false; kk = 0; kk = '';
    console.log('ok');
}
if ( (a>=b) && (a1==0) || (a3 == 'str') ){
    console.log(a);
};
```

# Сравнение без приведения типов(строгое)

```js
if (a1 === a2){ 
    console.log('сюда НЕ попадем');
}else{
   console.log('сюда попадем!!!');
}
```

# Сокращенная запись условия

```let <VAR> = <CONDITION> ? <VALUE-IF-TRUE> : <VALUE-IF-FALSE>;```
пример:
```js
let t45 = ( a1 == a2 ? 9384 :  6373 );
// тоже самое
let t45;
if (a1 === a2){ 
    t45 = 9386;
}else{
    t45 = 6573;
}
```

# Функции
```function <NAME>([<ARG1>,<ARG2>,...]){...}```

пример:
```js
function myfunc(a){
    console.log(a);
}
```
# Стрелочные ф-ции
```const <NAME> = ([<ARG1>,<ARG2>,...]) => {...}```

пример:
```js
const myfunc=(a)=>{
    console.log(a);
}
```



# Массивы
```js

let r = [1,2,3,4,5];
console.log(r[0]);// вывод первого элемента

// перебор
for(let i = 0; i<r.length; i++){
    console.log(r[i]);
};
```

фуункциональный способ перебора
```js
r.map((value,i)=>{
    console.log(value);
});

```
# Обьекты
```
let <OBJECT-NAME> = {
    <NAME>:<VALUE>,  // свойство
    ..,
    ..,
    <FUNC_NAME>([<ARG>]){  // метод - ф-ция
    },    
}
```
пример объекта:
```js
let o1 = {
    name:'string',
    age:56,
    eat(food){
 
    },
    sleep(delay){
 
    }
 };

 console.log(o1.name);
 console.log(o1.sleep(10));
```

# Классы 
```
 class <CLASSNAME> {

   constructor(){
      this.<NAME1> = <VALUE1>;  // свойство класса
      this.<NAME2> = <VALUE2>;
      ...
    }
    ..
    <FUNC_NAME>([<ARG>]){       // метод класса
    }    
}
```

пример:
```js
class Cat{
    constructor(){
        this.name = '';
        this.age = 0;
    }
    eat(food){

    }
    sleep(delay){

    }
};

let cat1 = new Cat();
let cat2 = new Cat();

```