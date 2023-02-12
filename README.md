# Команды git

0. git clone ADDR PATH - клонировать проект с github 
   ADDR - адрес прокета
   PATH - папка на компьютере куда скопируется проект

1. git pull origin main  - скачать с github
... изменили проект
2. git add . -  индексируем (предварительно сохраняем)
3. git commit -m "краткий комментарий"  - коммит, конечная фиксация
4. git push origin main - отправка кода на github

...
5. git status - посмотреть текущий статус проекта

# Переменные
let <NAME> [= <VALUE>];
Ex: 
let a = 10;
let b;
 
 # Типы переменных
 let a1 = 10;
let a2 = '10';
let a3 = "kaewjhfewkj";
let a4 = `qwkejfew
welkfewrf
werferwfj
werferwf`;
let a5 = true;
let a6 = false;
let a7 = null;
let a8 = undefined;

# Сравнение

let r; // let r = undefined;
let kk = undefined;

if (kk == r){ // kk = null; kk = false; kk = 0; kk = '';
    console.log('ok');
}
if ( (a>=b) && (a1==0) || (a3 == 'str') ){
    console.log(a);
};

# Сравнение без приведения типов(строгое)
if (a1 === a2){ 
    console.log('сюда НЕ попадем');
}else{
   console.log('сюда попадем!!!');
}

# Shugar cond
let <VAR> = <CONDITION> ? <VALUE-IF-TRUE> : <VALUE-IF-FALSE>;

let t45 = ( a1 == a2 ? 9384 :  6373 );

let t45;
if (a1 === a2){ 
    t45 = 9386;
}else{
    t45 = 6573;
}

# функции

function <NAME>([<ARG1>,<ARG2>,...]){
   ...
}

const <NAME> = ([<ARG1>,<ARG2>,...])=>{

}

# массивы
let r = [1,2,3,4,5];
for(let i = 0; i<r.length; i++){
    console.log(r[i]);
};
console.log(r[0]);// вывод первого элемента

let culc = (value,i)=>{
    console.log(value);
}; 
r.map(culc);

r.map((value,i)=>{
    console.log(value);
});

# классы\обьекты
let <OBJ> = {
    <NAME>:<VALUE>,
    ..
    <FUNC_NAME>([<ARG>]){
    },    
}
Ex:
let o1 = {
    name:'string',
    age:56,
    eat(food){
 
    },
    sleep(delay){
 
    }
 };

 class <CLASSNAME> {
   constructor(){
      this.<NAME1> = <VALUE1>;
      this.<NAME2> = <VALUE2>;
      ...
    }
    ..
    <FUNC_NAME>([<ARG>]){
    }    
}

Ex:
class Cat{
    constructor(){
        this.name = '';
        this.age = 0;
    }
    eat(food){

    }
    sleep(delay){

    }
}
let cat1 = new Cat();
let cat2 = new Cat();