# 14.longest_common_prefix
java
class Solution {
    public String longestCommonPrefix(String[] strs) {
       if(strs.length==0) return "";
        String sol=strs[0];
        for(int i=0;i<strs.length;i++){
           while(strs[i].indexOf(sol)!=0){
               sol=sol.substring(0,sol.length()-1);
           } 
        }
        return sol;
    }
}
