class Solution {
public:
    void setZeroes(vector<vector<int>>& matrix) {
        if(matrix.empty() || matrix[0].empty()) return;
        int nrow = matrix.size(), ncol = matrix[0].size();
        
        vector<pair<int,int>> zeros;
        
        for(int i = 0; i < nrow; i++){
            for(int j = 0; j < ncol; j++){
                if(matrix[i][j] == 0){
                    zeros.push_back({i,j});
                }else{
                    continue;
                }
            }
        }
        
        for(auto &ele : zeros){
            int row = ele.first;
            int col = ele.second;
            
            for(int i = 0; i < nrow; i++){
                matrix[i][col] = 0;
            } 
            
            for(int j = 0; j < ncol; j++){
                matrix[row][j] = 0;
            } 
        }
        
    }
};
