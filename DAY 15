class Solution {
public:
    int firstUniqChar(string s) {
        vector<int> oc(26);
        //store frequency of each character of s
        for (auto i : s) oc[i - 'a']++;
        //first character with frequency = 1 is the answer
        for (int i = 0; i < s.size(); i++) {
            if (oc[s[i] - 'a'] == 1) return i;
        }
        //no character with frequency = 1
        return -1;
    }
};
