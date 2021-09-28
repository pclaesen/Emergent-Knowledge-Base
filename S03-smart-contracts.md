### Question
I'm getting a compiler error like this:
error: "Source file requires different compiler version (current compiler is 0.8.4). How can I solve this incompatibility error?

### Answer
Check your truffle-config.js file and manually change the compiler version like so:

		
	module.exports = {
		compilers: {
			solc: {
				version: "^0.8.4", 
			}
		},
		...
	}
		
  
  You can find more information <a href="https://www.trufflesuite.com/docs/truffle/reference/configuration">here (official Truffle docs).</a>
	
If you're still getting an error in your .sol file on the pragma declaration, you can right-click the line of code and select `Solidity - Change workspace compiler version`.
