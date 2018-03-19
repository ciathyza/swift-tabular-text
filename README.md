# swift-tabular-text
A util class which can be used to output text as tables.

### Usage

Example:

```
let table = TabularText(2, true, "", " ", "", 120, ["Property", "Value"])
let mirror = Mirror(reflecting: self)
mirror.children.forEach
{
	child in
	if let label = child.label
	{
		table.add([label, "\(child.value)"])
	}
}
print(table.toString())
```

Output:

```
Property                  Value                                    
-------------------------------------------------------------------
appID                     com.ciathyza.AutumnDemo                  
appName                   AutumnDemo                               
debug                     false                                    
isStagingBuild            true                                     
logInstructions           true                                     
loginAttemptsDelay        2                                        
maxLoginAttempts          4                                        
maxScenarioRetries        1                                        
networkLoginTimeout       20                                       
networkRequestTimeout     20                                       
projectName               Autumn                                   
slowSeconds               0                                        
viewPresentTimeout        5                                        
viewReadyTimeout          15                                       
```
