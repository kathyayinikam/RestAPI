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
	}
```
Printing Even numbers
```
@GetMapping("/util/even/{limit1}")
	public ArrayList<Integer> getEven(@PathVariable int limit1){
		
		ArrayList<Integer>even1=new ArrayList<>();
		for(int i=0;i<limit1;i++) {
			if(i%2==0) {
				even1.add(i);
			}
		}
		return even1; 
	}
```
 Printing Ascii values
 ```
@GetMapping("/util/ascii")
	public String getAscii1() {
		String temp1="";
		for(int i=65;i<(65+26);i++) {
			temp1=temp1+i+"-->"+(char)i;
			
		}
		return temp1;
	}
