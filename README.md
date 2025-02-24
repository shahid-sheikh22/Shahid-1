# Basic Subject Calculator

Most basic code for calculating the pass or fail status of 4 subject.........

#include <stdio.h>
int main() {
    int marks[4], i;
    int passing_marks = 40; // Define passing criteria
    int pass = 1; // Assume pass initially
    for(i = 0; i < 4; i++) {
        printf("Enter marks for subject %d: ", i + 1);
        scanf("%d", &marks[i]);
        if(marks[i] < passing_marks) {
            pass = 0; // Mark as fail
        }
    }
    if(pass)
        printf("Pass\n");
    else
        printf("Fail\n");
    return 0;
}
