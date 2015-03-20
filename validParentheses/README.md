 #Data Structure:
 
     char Arrays, stack
  
 #Analyze:
  
     look up ASCII table, find that '(' 40
                                    ')' 41
                                    '[' 91
                                    ']' 93
                                    '{' 123
                                    '}' 125
      difference of every 2-character valid combination is 1 or 2 
      difference of invalid combination (ex.(] or {{) is larger than 2 or equal to 0
      
      and to pair valid character, use a stack, if pair successfully, remove parentheses, else add it to stack
      ex. ()[]{}
      empty=> add=> stack'('=> ')' - 'peek of stack'=1  => valid => remove => empty
      empty=> add=> stack'['=> ']' - 'peek of stack'=2  => valid => remove => empty
      empty=> add=> stack'{'=> '}' - 'peek of stack'=2  => valid => remove => empty => return true
      
      ex. ([)]
      empty=> add=> stack'('=>'['-'peek of stack'>2=> invalid=> add=> stack'(['
      ')'-'peek of stack'>2=> add=> stack'([)'
      ']'-'peek of stack'>2=> add=> stack'([)]'=> return false
      
 #Time Complexity:
   
     O(n)
     
 #Pseudocode:
 
      new stack;
      for(each character in the string){
         if(stack is empty or difference of cur with peek is larger than 2 or equal to 0) stack.push(cur);
         if(diffrence of cur and peek is equal to 2 or equal to 1) stack.pop();
      }
      return stack is empty
  
