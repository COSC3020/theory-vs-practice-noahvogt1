# Theory vs. Practice
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

I talked to some kid in class about this and I don't know his name, we just bounced ideas off each other.

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis ignores constants which doesn't give you the full
     realistic performance in practice.
  2. Asymptotic analysis also does not take into accound lower order terms,
     this can drastically change runtimes in pracitce. Just because a higher
     order term is $n^2$ does not mean that an extra 20n doesn't count towards
     runtime in practice.
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

  1. There may be hardware limits that will allow the program to run quickly on
     small element sizes (less than 2000 for example) but the ram/cache could be used up on
     larger sizes (greater than 2000 for example)
  2. A poorly balanced binary search tree (you say that it is a binary search tree on line 19
     of this markdown file) could also produce bad timing. If the one with 1,000 elements
     was well balanced and the 10,000 element one was poorly balanced, then the 10,000
     element one would have a runtime closer to a linked list which would be anywhere from 6.66
     seconds all the way to 1.4 hours depending on how poorly balanced the tree was. Math below:
     One step is considered to be one step down the tree towards the item.

     $log_2(1000) = 10$  steps in 5 seconds, this is aproximatly 1 step every half second.

     10,000 steps in a linked list would then take  $10000 * 0.5 = 5000$  seconds

     Convert this to hours:  $5000 / 3600 = 1.4$  hours. This runtime can not be exact but is
     a good approximation of the max runtime because it represents what a linked list form of a
     tree would be. So in this case the runtime was not so out of balance that it was a linked list.
     This is because the runtime was not 1.4 hours, it was 100 seconds. This means that the binary
     search tree was out of balance but not terribly.
     
     We know the depth of the tree was aproximatly $log_2(1000) = 10$ and this took five seconds. We
     can then solve for the depth of out of balance tree. (10/5s) = (x/100s), x = 200. Therefor the
     tree depth must be closer to 200. This means that the data is far from a linked list but is still
     terribly out of balance which accounts for the bad runtime.
     
  3. There could be background software running at the time you run the large element
     list but when you ran it on the smaller list size the background tasks weren't running

Add your answers to this markdown file.
