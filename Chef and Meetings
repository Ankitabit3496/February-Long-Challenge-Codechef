#include<bits/stdc++.h>
using namespace std;

int hourhand(string s, int t)
{
    int hour;
    hour = 10 *(s[0 + t] - '0') + 1* (s[1 + t] - '0');
    
    if(s[6 + t] == 'P'){
        if(hour != 12) {
            hour += 12;
        }
        
    }
    if(s[6 + t] == 'A') {
        if(hour == 12){
        hour-= 12;
        }
    }
    return hour;
}

int minutehand(string s, int t)
{
    int minute;
    
    minute = 10 *(s[3 + t] - '0') + (s[4 + t] - '0');
    
    return minute;
}

int main()
{
    long long  t;
    cin>>t;
    cin.ignore();

    while(t--)
    {
        string s; 
        getline(cin,s);
        int hour = hourhand(s, 0);
        int minute = minutehand(s, 0);
     
        long long int n;
        cin>>n;
        cin.ignore();
        
        string t = "";
        while(n--)
        {
            string p; 
            getline(cin,p);
            int u = hourhand(p, 0);
            int v = minutehand(p, 0);
            int w = hourhand(p, 9);
            int z = minutehand(p, 9);

            if((u>hour)||(w<hour)) {
                t.push_back('0');

            }
            else if(u == hour && v> minute){
               t.push_back('0');
            }
            else if(w == hour && z< minute) {
                t.push_back('0');
            }
            else {
                t.push_back('1');
                
            }
        }
        
        cout<<t<<"\n";       
    }
    return 0;
}
