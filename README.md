# RestAPI
Factorial
```
	@GetMapping("/util/factorial/{num1}")
	public String fact1(@PathVariable int num1) {
		
		int fact1=1;
		for(int i=num1;i>0;i--) {
			fact1=fact1*i;
		}
		return num1+" --> "+fact1; 
	}```
