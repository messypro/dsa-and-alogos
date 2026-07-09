Reach for binary search when you see:
 - sorted array
 - find an element/position/boundary
 - O(log n) is hinted or expected
 - A monotonic search space - some condition flips from false → true exactly once

Cut the search space in half every step. Instead of scanning n elements, you do it in ~log₂(n) steps.


Template 

```
int left=0, right =arr.length-1;

while(left <=right){ // <= is important! left + right can overflow int
  int mid = left + (right -left)/2;

if(arr[mid] == target){

  return mid;

} else if(arr[mid] < target){
    left = mid+1;


} else{

right = mid -1;

}

}

return -1;


```

<img width="807" height="348" alt="Screenshot 2026-07-09 at 4 12 21 PM" src="https://github.com/user-attachments/assets/d8d96462-ed67-470c-804c-fa49206bf802" />


