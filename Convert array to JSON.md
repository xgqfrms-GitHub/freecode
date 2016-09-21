# Convert array to JSON



[http://stackoverflow.com/questions/2295496/convert-array-to-json](http://stackoverflow.com/questions/2295496/convert-array-to-json)



```javascript
    function fib(n){
	    var b = 1;
    	var tmp_var = 0;
	    var result = [];
        for (var a = 0; a < n; a++) {
        	result.push(a)
        	// console.log("a = " + a + ",\n");
        	tmp_var = b;
        	// console.log("tmp_var = " + tmp_var + ",\n");
        	b += a;
        	// console.log("b = " + b + ",\n");
           a = tmp_var-1;
        }
        var JsonString = JSON.stringify(result);
        console.log("JsonString  = " + JsonString  + ",\n");
    }
    fib(10);
```