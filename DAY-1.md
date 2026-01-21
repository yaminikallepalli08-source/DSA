Missing Number in an Array:
```  class Solution {
    int missingNum(int arr[]) {
        long sum=0;
        for(int i=0;i<arr.length;i++)
        {
            sum+=arr[i];
        }
        long n=arr.length+1L;
       long t=n*(n+1)/2;
       
      return  (int)(t-sum);  
    }
} 
```
