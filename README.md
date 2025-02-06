# Theory vs. Practice
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

I talked to some kid in class about this and I don't know his name, we just bounced ideas off each other.

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis ignores constants which doesn't give you the full
     realistic performance in practice.
  2. Asymptotic analysis assumes very large inputs; however, in practice a smaller
     input size might run better on theoretically worse algorithms. Take two functions:
     $f(n) = n$ and $g(n) = n^2/16$
  4. There are limits in terms of hardware as well, so it could run faster on
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

  1. There may be hardware limits that will allow the program to run quickly on
     small element sizes (less than 2000 for example) but the ram/cache could be used up on
     larger sizes (greater than 2000 for example)
  2. A poorly balanced binary search tree (line 18) could also produce bad timing
  3. There could be background software running at the time you run the large element
     list but when you ran it on the smaller list size the background tasks weren't running

Add your answers to this markdown file.
