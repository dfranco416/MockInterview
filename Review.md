 
 ## Mock Interview Analysis
 
 When reviewing the interview I saw that
 my strengths of the interview were:
 
 > I felt comfortable when talking about not technical topics such as how I got to this point and willingness to continue  
 > Taking a short moment to think about my answers
 
 My weaknesses were:
 > Technical terms  
 > I did not do well when unsure of answer.  
 > I froze up when I was not confident in an answer even if I normally would've known the answer  
 > I did not attempt hard enough to solve the technical parts on my own
 
 
 **Below is the coding challenge that I was given:**  
 *The question was:*  
 Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.  
   
 **Here is the answer that I came up with after the interview**  
 ``` Java
 class Solution {
    public void moveZeroes(int[] nums) {
        
        int count = 0;
        
        for(int i = 0; i < nums.length; i++){
            if(nums[i] != 0){
                // nums[count++] = nums[i];
                int temp = nums[i];
                nums[i]= nums[count];
                nums[count] = temp;
                count++;
            }
        }
       
    }
}
 
 ```
