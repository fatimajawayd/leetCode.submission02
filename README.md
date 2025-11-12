# LeetCode.submission02

## PROBLEM:01
### MOVE ZEROES AT THE END OF AN ARRAY
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

## PROBLEM:02
### REVERSING STRING
```c
#include <stdio.h>

void reverseString(char* str, int sSize){
    for(int i =0; i<sSize/2; i++){
        char temp = str[i];
        str[i] = str[sSize-1-i];
        str[sSize-1-i] = temp;
    }
}
int main(){
    char str[] = {'H', 'e', 'l', 'l', 'o'};
    int sSize = sizeof(str)/sizeof(str[0]);

    printf("After reversing the string:\n");
    reverseString(str, sSize);
    for(int i=0; i<sSize; i++){
        printf("%c ", str[i]);
    }
    printf("\n");
    return 0;

}

```

## PROBLEM:03
### REMOVING DUPLICATES
```c

```
