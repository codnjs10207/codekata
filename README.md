# codekata

n을 x로 나눈 나머지가 1이 되도록 하는 가장 작은 자연수 x를 return

#include <stdio.h>
#include <stdbool.h>
#include <stdlib.h>

int solution(int n) {
    int answer = 0;
    for (int i = 1; i < n; i++) {
        if (n % i == 1) 
        {
            answer = i;
            break;
        }
    }
    return answer;
}