#include <bits/stdc++.h>
using namespace std;

typedef long long ll;
typedef vector<int> vi;

#define IOS                  \
    ios::sync_with_stdio(0); \
    cin.tie(0);              \
    cout.tie(0);
#define fr first
#define sc second
//#define endl "\n"
#define input_arr(a, n)         \
    for (int i = 0; i < n; i++) \
        cin >> a[i];
#define f(i, x, n) for (ll i = x; i < n; i++)

int main()
{
    IOS;
    int tc = 1 ;
    //cin >> tc;
    while(tc--)
    {
        ll n ;
        cin >> n;
        bool prime[n + 1];
        memset(prime, true, sizeof(prime));

        for (int i = 2; i*i<= n; i++)
        {
            if (prime[i] == true)
            {
                for (int j =i*i ; j <= n; j+=i )
                    prime[j] = false;
            }
        }
        vector<int> prm ;
        for (int i = 2; i <= n; i++)
            if (prime[i])
                prm.push_back(i) ;
        cout<<"Following are the prime numbers: " ;
        for(int &i : prm)
            cout<< i <<" " ;
        cout<< "\n" ;
    }
    return 0;
}
