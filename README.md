#include <iostream>
using namespace std;

bool isPalindrome(int x) {
    int rem,reverse=0;
    while(x!=0){    
        rem=x%10;      
        reverse=reverse*10+rem;    
        x/=10;
        if (x == reverse) return true;
        else return false;
    }
    return true;
}

int main() {
    int n;
    cin >>n;
    
    if(isPalindrome(n)) {
        cout <<n<<" is a palindrome";
    }
    else {
        cout << n<<" is NOT a palindrome";
    }
    return 0;
}
