
//brute force

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        vector <int> temp;
        for(int i=0 ; i<nums.size();i++){
            for(int j=i+1;j<nums.size();j++){
                if(nums[i]+nums[j]==target){
                    temp.push_back(i);
                    temp.push_back(j);
                    return temp;
                }
            }
        }
        return temp;
    }
};

//Optimum with maps

class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        vector<int>temp;
        int diff;
        unordered_map<int,int> m;
        for(int i=0;i<nums.size();i++){
            diff=target-nums[i];
            if(m.find(diff) != m.end() && m.find(diff)->second != i){
                temp.push_back(i);
                temp.push_back(m.find(diff)->second);
                return temp;
            }
            m[nums[i]]=i;
        }
        return temp;
    }
};


