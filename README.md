# 450Questions

## Reverse a String 

### O(n)

```cpp
#include <iostream>
using namespace std;

int main() {
        
        int t;
        cin>>t;
        while(t--)
        {
            string s;
            cin>>s;
            
            int n=s.size();
            int i=0;
            int j=n-1 ;
            while(i<j)
            {
                char c=s[i];
                s[i]=s[j];
                s[j]=c;
                ++i;
                --j;
            }
            cout<<s<<"\n";
        }
    
	return 0;
}
```

## Middle of three

```cpp
// { Driver Code Starts
//Initial template for C++

#include <bits/stdc++.h>
using namespace std;

 // } Driver Code Ends


//User function template for C++

class Solution{
  public:
    int middle(int A, int B, int C){
        if(A>B)
        swap(A,B);
        if(C<B)
        swap(C,B);
        if(A>B)
        swap(A,B);
        return B ;
        
    }
};

// { Driver Code Starts.
int main()
{
    int t;
    cin>>t;
    while(t--)
    {
        int A,B,C;
        cin>>A>>B>>C;
        Solution ob;
        cout<<ob.middle(A,B,C) <<"\n";
    }
    return 0;
}  // } Driver Code Ends
```

## Kth Smallest Element

## O(N*log(N))

```cpp
#include <iostream>
#include<bits/stdc++.h>
using namespace std;

int main() {
	
	int t;
	cin>>t;
	while(t--)
	{
	    int n ;
	    cin>>n;
	    int a[n];
	    for(int i=0 ; i<n ; ++i)
	    cin>>a[i];
	    int k;
	    cin>>k ;
	    sort(a,a+n);
	    cout<<a[k-1]<<"\n";
	}
	
	
	return 0;
}
```

