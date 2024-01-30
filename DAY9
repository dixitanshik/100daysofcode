
class Solution {

    long resolves(int a, int b, char Operator){
        if(Operator == '+') return a + b;
        else if(Operator == '-') return a - b;
        else if(Operator == '*') return (long)a*b;
        return a/b;
    }
public:
    int evalRPN(vector<string>& tokens) {
        stack<long> Stack;
        int n = tokens.size();
        for(int i = 0; i < n; i++){

            if(tokens[i].size() == 1 and tokens[i][0] < 48){
                long integer2 = Stack.top();
                Stack.pop();
                long integer1 = Stack.top();
                Stack.pop();
                
                string Operator = tokens[i];
                long resolvedAns = resolves(integer1, integer2 , Operator[0]);
                Stack.push(resolvedAns);
            }else 
                Stack.push(stol(tokens[i]));
        }
        return Stack.top();
    }
};

