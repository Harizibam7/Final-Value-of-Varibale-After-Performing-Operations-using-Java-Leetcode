# Final-Value-of-Varibale-After-Performing-Operations-using-Java-Leetcode
    class Solution {
        public int finalValueAfterOperations(String[] operations) {
            int x =0;
            char opr = '+';
            for(int i =0; i<operations.length;i++){
                if((operations[i].charAt(0)==opr) || (operations[i].charAt(operations[i].length()-1) == opr)){
                    x = x+1;   
                }else{
                    x = x-1;
                }
                
            }
            return x;
        }
    }
