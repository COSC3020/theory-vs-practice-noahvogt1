# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis ignores constants which doesn't give you the full
     realistic performance in practice.
  2. Nothing is ever actually run to the point of asymptotic analysis, you may
     itterate a function over 100,000 elements but it is still not as high as
     you would need to go to reach asymptotic. Therefor it doesn't accuratly
     represent what would happen in practice
  3. There are limits in terms of hardware as well, so it could run faster on
     a super computer compared to a raspberry pi.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  $xlog_2(1000)=5$
  
  $10x=5$ Roughly
  
  $x=2$
  
  $2log_2(10000) = 6.66$
  
  It would take roughly 6.66 seconds using the time complexity.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. Again there are hardware limits that could have produced a worse time.
  2. A poorly balanced tree could also produce bad timing
  3. 

Add your answers to this markdown file.
