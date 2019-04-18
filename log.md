**This file is used to record the problems and the targets of this project.**



4.18

- problems : 

1. Can not get the `keys` of the element at a stack-layout, which is aimed to show the type of the disaster.
- targets : 
1. Fix problem 1
2. Add many interactive events

Problem 1 has been fixed by a very low method : 

```javascript
function getKeys(d) {
			return series[parseInt(groups.selectAll("rect").data().indexOf(d) / series[0].length)].key;
		}
```

The process of finding this method is Brute-force, by using the chrome's console to see every result of a paragraph of code, like `groups.selectAll("rect").data()`.

I have to say that the chrome's console is so powerful!
