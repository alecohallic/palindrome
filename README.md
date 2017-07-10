# palindrome
Javascript function that logs whether a parameter is a palindrome or not

  function palindrome(word){
      var half1= word.slice(0,word.length/2);
        if(word.length % 2 !==0){
        half1 = word.slice(0,(word.length/2)+1).toUpperCase();
        }
      
      var half2 = word.slice(word.length/2,word.length);
      var brokenHalf = half2.split("");
      var brokenreverse = brokenHalf.reverse();
      var cba = brokenreverse.join("").toUpperCase();
    
      
      if(cba == half1){
        console.log("It's a palindrome");
      }
      else{
        console.log("Not a palindrome")
      }
  }

    palindrome("lEvel");
