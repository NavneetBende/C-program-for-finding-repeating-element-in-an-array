#include<stdio.h>
// Time Complexity : O(n^2)
// O(n^2) : sort the array and O(n) to count repeating


// using bubble sort to sort the array
// you can use a better sorting algorithm to reduce 
// time complexity to O(n log n) to sort
int bubbleSort(int arr[], int size){
    for (int i = 0; i < size-1; i++){       

    // Since, after each iteration righmost i elements are sorted   
    for (int j = 0; j < size-i-1; j++) if (arr[j] > arr[j+1]) 
        {
            int temp = arr[j]; // swap the element
            arr[j] = arr[j+1]; 
            arr[j+1] = temp; 
        }
    }
}

// find repeating element
void findRepeating(int arr[], int n){
    // Traverse the sorted array
    // arr = {3, 10, 10, 11, 20, 20, 30, 30}
    
    int count = 0;
    // this step may look like O(n^2) but its actually O(n)
    // look closely, we traverse every element only once
    for (int i = 0; i < n; i++) {
        
        int flag = 0;
        
        // Move the index ahead whenever you encounter duplicates
        while (i < n - 1 && arr[i] == arr[i + 1]){
            // indicates that we have found duplicate
            flag = 1;
            i++;
        }
        // since i++ happened, we need to print previous element
        if(flag)
            printf("%d, ",(arr[i-1]));
    }
 
    return;
    
}

// Main function to run the program
int main() 
{ 
    int arr[] = {20, 30, 10, 2, 10, 20, 30, 11}; 
    int n = sizeof(arr)/sizeof(arr[0]);
    
    bubbleSort(arr, n);
    
    findRepeating(arr, n);
 
   return 0; 
}
// Time Complexity : O(N)
// Space Complexity : O(1)
