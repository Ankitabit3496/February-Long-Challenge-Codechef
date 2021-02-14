//Partially Accepted, TLE in one test case.

#include <bits/stdc++.h>
using namespace std;

int main() {
   ios_base::sync_with_stdio(false);
   cin.tie(NULL);
   
    int t;
    cin>>t;
    vector<int>c;
    while(t--){
        
        int n;
        cin>>n;
        set<string>v;
        int count=0;
        int x=0;
        
        while(x<n){
            string k;
            cin>>k;
            v.insert(k);
            x++;
        }
        set<string>::iterator i=v.begin(),j;
        
        for(i; i!=v.end(); i++){
            for(j = i; j!=v.end(); j++){
               
               string s1 = *i;
               string s2 = *j;
               
               if(s1[0]!=s2[0]){
                   string p1 = s1;
                   p1[0]= s2[0];
                   string p2 =s2;
                   p2[0]= s1[0];
                   
                   if(v.find(p1)==v.end() && v.find(p2)==v.end()){
                       count = count+2;
                   }
                   
               }
               
            }
        }
        cout<<count<<'\n';
    }
    
	return 0;
}
