#include<iostream>
#include<vector>
#include<algorithm>

using namespace std;

//int main() 안에 vector 선언하면 시간 초과(왜?)
//다른 함수의 매개변수로 vector 전달하면 시간 초과(왜?)
vector<int> target; 

void binarySearch(int num){
    int start = 0, end = target.size() - 1, mid;
    while(start<=end){
        mid = (start + end)/2;
        if(num == target[mid]){
            printf("1\n");
            return;
        } else if(num > target[mid]){
            start = mid + 1;
        } else{
            end = mid - 1;
        }
    }
    printf("0\n");
}

int main() {
    int t, m, num;
    scanf("%d", &t);
    for(int i = 0; i < t; i++){
        scanf("%d", &num);
        target.push_back(num);
    }
    sort(target.begin(), target.end());
    scanf("%d", &m);
    for(int i = 0; i < m; i++){
        scanf("%d", &num);
        binarySearch(num);
    }
}
