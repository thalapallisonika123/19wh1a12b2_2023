class Solution {
public:
    bool isValid(string s) {
        int n = s.length();
        int i;
        stack<char>stk;
       
        for(i=0;i<n;i++)
        {
            if(s[i]=='('||s[i]=='{'||s[i]=='[')
            {
                stk.push(s[i]);
            }
            else if(stk.empty()&&s[i]==')'||stk.empty()&&s[i]=='}'||stk.empty()&&s[i]==']')
            {
                return false;
            }
            else if(s[i]==')'&&stk.top()=='(')
            {
                stk.pop();
            }
           else if(s[i]=='}'&&stk.top()=='{')
            {
               stk.pop();
            }
            else if(s[i]==']'&&stk.top()=='[')
            {
                stk.pop();
            }
            else
            {
                return false;
            }
        
        }
        
        if(stk.empty())
        {
            return true;
        }
        
        return false;
        
        
    }
};
