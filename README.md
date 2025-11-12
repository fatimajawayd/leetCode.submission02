# LeetCode.submission02

## PROBLEM:01
### MOVE ZEROES TO THE END OF AN ARRAY
```c
#include <stdio.h>

void removeZero(int* nums, int numsSize){
    int nonZero = 0;
    for(int i=0; i<numsSize; i++){
        if(nums[i] != 0){
            nums[nonZero++] = nums[i];
        }
    }
    while(nonZero<numsSize){
        nums[nonZero++] = 0;
    }
}
int main(){
    int nums[] = {0, 1, 0, 2, 4};
    int numsSize = sizeof(nums)/sizeof(nums[0]);

    removeZero(nums, numsSize);

    printf("After moving zeroes at the end:\n");
    for(int i=0; i<numsSize; i++){
        printf("%d ",nums[i]);
    }
    printf("\n");
    return 0;
}
```
