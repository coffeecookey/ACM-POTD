## Solution
```
class Solution {
public:
    int removeDuplicates(vector<int>& nums) {

        if(nums.size()==0) return 0;
        int k = 1;
        for(int i=1;i<nums.size();i++){
            if(nums[i] != nums[i-1]){
                nums[k] = nums[i];
                k++;
            }
        }
        return k;
    }
};
```

<img width="1440" height="900" alt="Screenshot 2026-03-23 at 00 34 57" src="https://github.com/user-attachments/assets/6ef38f34-d424-46c4-a3ea-91e81b957c1b" />
