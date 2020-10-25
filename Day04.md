作业1

```
const tipCalculator = bills => {
const tips = []
const costs = []
bills.forEach(bill =>{
let tip;
if (bill < 50){
tip = bill * 0.2
}else if (bill >= 50 && bill < 200){
tip = bill * 0.15
}else{
tip = bill * 0.1
}
const cost = bill + tip
tips.push(tip)
costs.push(cost)
})
console.log(tips,costs)
}
tipCalculator([124,48,268])
```

作业2

```
function mean1() {
    var l=arguments.length;
    var sum=0;
    for(var i=0;i<=l;i++){
        sum+=i;
    }
    var Avg=sum/l;
    console.log(Avg);
}
mean1(1,2,3,4);
```

