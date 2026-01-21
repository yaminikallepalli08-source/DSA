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
Second Largest  in ana Array
```class Solution {
    
    public int getSecondLargest(int[] arr) {
        int big=arr[0];
        int secbig=Integer.MIN_VALUE;
        for(int i=0;i<arr.length;i++){
            if(arr[i]>big)
            {
                 secbig=big;
                big=arr[i];
            }
            else if(arr[i]>secbig && arr[i]!=big){
                secbig=arr[i];
            }
           
        }
      return secbig;
```
        
    }
}
