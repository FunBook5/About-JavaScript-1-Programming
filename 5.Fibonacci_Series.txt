function fibonacciGenerator (n) {
    
    const arr=[];
    var x = 0;
    var num1 = 0;
    var num2 = 1;
    
    if(n==1){
        return '0';
    }
    
    if(n==2){
    arr[0]=0;
    arr[1]=1;
        
        return arr;
    }
    
    
    for(var i=0;i<n;i++){
         arr[i] = x;
         
         x = num1 + num2;
         num2 = num1;
         num1 = x;
         
    }
    
    return arr;
    
    
    
    
    
    //Return an array of fibonacci numbers starting from 0.
}