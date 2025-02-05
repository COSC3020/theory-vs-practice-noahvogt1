# Theory vs. Practice
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

I talked to some kid in class about this and I don't know his name, we just bounced ideas off each other.

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis ignores constants which doesn't give you the full
     realistic performance in practice.
  2. Nothing is ever actually run to the point of an infinite size which is where
     asymptotic analysis is done, you may itterate a function over 100,000
     elements but it is still not as high as you would need to go to reach asymptotic.
     Therefor it doesn't accuratly represent what would happen in practice
  3. There are limits in terms of hardware as well, so it could run faster on
     a super computer compared to a raspberry pi.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  $xlog_2(1000)=5$
  
  $10x=5$ Roughly
  
  $x=(1/2)$
  
  $(1/2)log_2(10000) = 6.66$
  
  It would take roughly 6.66 seconds using the time complexity.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. Again there are hardware limits that could have produced a worse time.
  2. A poorly balanced tree could also produce bad timing
  3. There could be background software running at the time causing slow runtimes

Add your answers to this markdown file.
