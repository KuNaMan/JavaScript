# Day02作业



## 作业01

Mark和John在PK他们的BMI（Body Mass Index，体重指数）。

体重指数是用这个公式计算的：
$$
BMI = mass / height^2 = mass / (height * height)。
$$
其中，mass是体重，单位为kg；height为身高，单位为米。

请用 JavaScript 编写一个程序，命名为 `bmi.js` ，完成如下任务：

1. 用变量存储Mark和John的体重以及身高；

2. 计算二人的BMI；

3. 创建一个布尔变量，用来包含Mark的BMI是否比John更高；

4. 打印一个字符串到控制台，包含第三步的变量（比如"Mark的BMI是否比John更高？true"）

   ```
   //1.用变量存储Mark和John的体重以及身高；
   let M_height = 1.88,M_Mass = 70;
   let J_height = 1.82,J_Mass = 63;
   
   //2.计算二人的BMI；
   let M_BMI = M_Mass / (M_height * M_height);
   let J_BMI = J_Mass / (J_height * J_height);
   console.log("Mark的BMI值为:",M_BMI);
   console.log("John的BMI值为:",J_BMI);
   
   //3.创建一个布尔变量，用来包含Mark的BMI是否比John更高；
   let compare;
   compare = (M_BMI > J_BMI) ? true : false;
   console.log(compare);
   
   //4.打印一个字符串到控制台，包含第三步的变量（比如"Mark的BMI是否比John更高？true"）。
   console.log("Mark的BMI是否比John的更高？",String(compare));
   ```

   ![](C:\Users\11\AppData\Roaming\Typora\typora-user-images\image-20201010230215142.png)

## 作业02

John 和 Mike 都在不同的队打篮球。在最近的3场比赛中，John 的队得了89分、120分和103分，而 Mike 的队得了116分、94分和123分。

用 JavaScript 编写程序，存为 `ball.js`，完成以下任务：

1. 计算每队的平均分；
2. 决定哪支球队平均获胜（平均分最高），并将胜者打印到控制台。在输出中也包括平均分；
3. 然后改变分数来显示不同的赢家。别忘了考虑到可能会有平局（平均分相同）；
4. Mary 也打篮球，她的队得了97分、134分和105分。像前面一样，把平均分胜出者记录到控制台；
5. 像前面一样，改变分数以产生不同的赢家，记住可能会有平局。

```
//1.计算每队的平均分；
let JohnAvg = (89 + 120 + 103) / 3;
let MikeAvg = (116 + 94 + 123) / 3;
console.log("John的平均分是："+JohnAvg+"\n" +"Mike的平均分是："+MikeAvg+"\n")
//2.决定哪支球队平均获胜（平均分最高），并将胜者打印到控制台。在输出中也包括平均分；
if(JohnAvg > MikeAvg){    
    console.log("John是获胜队伍！" + "John的平均分是："+JohnAvg);
    }
else if (MikeAvg > JohnAvg){   
    console.log("Mike是获胜队伍！" + "Mike的平均分是："+MikeAvg);
    }
else{   
    console.log("平局！");
    }
//3.然后改变分数来显示不同的赢家。别忘了考虑到可能会有平局（平均分相同）；
let JohnAvg1 = (98 + 106 + 110) / 3;
let MikeAvg1 = (86 + 102 + 108) / 3;
console.log("John的平均分是："+JohnAvg1+"\n" +"Mike的平均分是："+MikeAvg1+"\n")
if(JohnAvg1 > MikeAvg1){    
    console.log("John是获胜队伍！" + "John的平均分是："+JohnAvg1);
    }
else if (MikeAvg1 > JohnAvg1){    
    console.log("Mike是获胜队伍！" + "Mike的平均分是："+MikeAvg1);
    }
else{   
    console.log("平局！");
    }
//4.Mary 也打篮球，她的队得了97分、134分和105分。像前面一样，把平均分胜出者记录到控制台；
let JohnAvg2 = (89 + 120 + 103) / 3;
let MikeAvg2 = (116 + 94 + 123) / 3;
let MaryAvg2 = (97 + 134 + 105) / 3;
console.log("John的平均分是："+JohnAvg2+"\n" +"Mike的平均分是："+MikeAvg2+"\n"+"Mary的平均分是："+MaryAvg2+"\n")
if((JohnAvg2 > MikeAvg2) && (JohnAvg2 > MaryAvg2)){    
    console.log("John是获胜队伍！" + "John的平均分是："+JohnAvg2);
    }
else if ((MikeAvg2 > JohnAvg2) && (MikeAvg2 > MaryAvg2)){   
    console.log("Mike是获胜队伍！" + "Mike的平均分是："+MikeAvg2);
    }
else if((MaryAvg2 > JohnAvg2) && (MaryAvg2 > MikeAvg2)){  
    console.log("Mary是获胜队伍！" + "Mary的平均分是："+MaryAvg2);
    }
else{   
    console.log("平局！");
    }
//5.像前面一样，改变分数以产生不同的赢家，记住可能会有平局。
let JohnAvg3 = (92 + 111 + 109) / 3;
let MikeAvg3 = (105 + 110 + 97) / 3;
let MaryAvg3 = (115 + 95 + 96) / 3;
console.log("John的平均分是："+JohnAvg3+"\n" +"Mike的平均分是："+MikeAvg3+"\n"+"Mary的平均分是："+MaryAvg3+"\n")
if((JohnAvg3 > MikeAvg3) && (JohnAvg3 > MaryAvg3)){    
    console.log("John是获胜队伍！" + "John的平均分是："+JohnAvg3);
    }
else if ((MikeAvg3 > JohnAvg3) && (MikeAvg3 > MaryAvg3)){   
    console.log("Mike是获胜队伍！" + "Mike的平均分是："+MikeAvg3);
    }
else if((MaryAvg3 > JohnAvg3) && (MaryAvg3 > MikeAvg3)){  
    console.log("Mary是获胜队伍！" + "Mary的平均分是："+MaryAvg3);
    }
else{   
    console.log("平局！");
    }
```

![](C:\Users\11\AppData\Roaming\Typora\typora-user-images\image-20201010235044417.png)

## 作业03

用JavaScript编写程序，取名 `star.js`，在控制台输出如下图形：

```
   *
  * *
 * * *
* * * *
 * * *
  * *
   *
```

```
let all ="";
for(let i=1; i<=4; i++){    
let blank = " ";    
let stars = " ";   
for(let m = 1; m <= 4-i; m++){
blank = blank + " ";
 }
for(let n=1; n<=i;n++){
 stars = stars + "*" + " ";
 }    
 all = all +blank + stars +"\n";
 }
 for(let i=4-1; i>0; i--){    
 let blank = " ";    
 let stars = " ";    
 for(let m=1; m<=4-i; m++){        
 blank += " ";    
 }    
 for(let n=1; n<=i; n++){        
 stars += "*" + " ";    
 }     
 all += blank + stars + "\n";}console.log(all);
```

![](C:\Users\11\AppData\Roaming\Typora\typora-user-images\image-20201010235428823.png)