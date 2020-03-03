3. function sumAndMultipl (a,b,c){
    var theSum = sum(a, sum(b,c)[0])[0];
    var Product = multiply(a, multiply(b,c)[0])[0];
    return [theSum, product,]
}

4. var theSum = sum(sumArr[0], sum(sumArr[1], sumArr[2]));

6. var testDynamicArray = [1,2,3,4,5];

function multiplyAnyArray(dynamicArray){

var product = 1;

for(var i =0; i < dynamicArray.length; i++){

    product += dynamicArray[i];

}
 
var message = 'The Numbers ';

for(var i = 0; j < dynamicArray.length; i++){

    message += dynamicArray[i];

if (i < dynamicArray.length -1) {
    message += ',';

}

}
message += ' have a product ' + product + '.';
return [product, message];
}


template literal - keep looking it up. seems difficult.

array stores information.   

_Object Literal_  
var objExample {  
    key : value;  
    'strings' : -whatever;  
    -[]  
    - function() - is a method;  

}  


