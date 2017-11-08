#include <iostream>
using namespace std;
 
unsigned long int bitstrings(int n)
{
    unsigned long int a[n], b[n];
    const unsigned int M = 1000000007;
    
    a[0] = b[0] = 1;
    
    for (int i = 1; i < n; i++)
    {
        a[i] = ((a[i-1]%M) +( b[i-1]% M))%M;
        b[i] = a[i-1]%M;
    }
    
    return a[n-1] + b[n-1];
}

int main()
{
    int t;
    cin>>t;
    int length[t];
    for(int i=0;i<t;i++)
    {
        cin>>length[i];
    }
    
    for(int j=0;j<t;j++)
    {
        cout<<bitstrings(length[j])<<"\n";
    }
    
    return 0;
}
