# Activity-13---Space-Constraints

 ##Question 1
There are two nested loops, so it creates about n² combinations.
  so space complexity = O(n²)

  ##Question 2
  If the input size is n, the new array is also size n.
    so = O(n)

  ##Question 3
   fucntion reverseInPlace(array) {
     let left = 0;
     let right = array.length -1;
  while (left < right) {
    let temp = array[left];
    array[left] = array[right];
    array [right} = temp;

    left++;
    right--;  
    }
      return array;
      }

  Space Complexity = O(1)

  ##Question 4

  | Version    | Time Complexity | Space Complexity |
| ---------- | --------------- | ---------------- |
| Version #1 | O(n)            | O(n)             |
| Version #2 | O(n)            | O(1)             |
| Version #3 | O(n)            | O(n)             |

Version 1 Work: 
function doubleArray1(array) { 
	let newArray = [];
  for(let i = 0; i < array.length; i++) { 
		newArray.push(array[i] * 2);
	}
	return newArray; 
}

Version 2 Work:
function doubleArray2(array) {
	for(let i = 0; i < array.length; i++) {
  	array[i] *= 2;
  }
	return array; 
}

Version 3 Work:
function doubleArray3(array, index=0) {
  if (index >= aarray.length) 
  { return;}
array[index] *= 2;
doubleArray3(array, index +1);
return array;
}


  
