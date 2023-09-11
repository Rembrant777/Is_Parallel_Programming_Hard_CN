# How To Use This Book 

The purpose of this book is to help you program shared-memory parallel systems without risking your sanity. 

Nevertheless, you should think of the information in this book as a fundation on which to build, rather than as a completed cathedral. Your mission, if you choose to accept, is to help make further progress in the exciting field of parallel programming -- progress that will in time render this book obsolete. 

Parallel programming in the 21-st century is no longer focused solely on science, research, and grand-challenge projects. And this is all to the good, because it means that parallel programming is becoming an engineering discipline. 

Therefore, as befits an engineering discipline, this book examines specific parallel-programming tasks and describes how to approach them. In some suprisingly common cases, these tasks can be automated. 

This book is written in the hope that presenting the engineering discipline underlying successful parallel-programming projects will free a new generation of parallel hackers from the need to slowly and painstakingly reinvent old wheels, enabling them to instead focus their energy and creativity on new frontiers. 


However, what you get from this book will be determined by what you put into it. It is hoped that simply reading this book will be helpful, and that working the Quick Quizzes will be even more helpful.

However, the best results come from applying the techniques taught in this book to real-life problems. As always, practice makes perfect. 

But no matter how you approach it, we sincerely hope that parallel programming brings you at least as much func, excitement, and challenge that it has brought to us!


## 1.1 Roadmap 

```
Cat: Where are you going ? 
Alice: Which way should I go ? 
Cat: That depends on where you are going. 
Alice: I don't know. 
Cat: Then it doesn't matter which way you go. 
```

And this book is a handbook of widely applicable and heavily used design techniques, rather than a collection of optimal algorithms with tiny areas of applicability. You are currently reading Chapter 1, but you knew that already. Chapter 2 gives a high-level overview of parallel programming. 

Chapter 3 introduces shared-memory parallel hardward. After all, it is difficult to write good parallel code unless you understand the underlying hardward. Because hardware constantly evolves, this chapter will always be out of date. We will nevertheless do our best to keep up. Chapter 4 then provides a very brief overview of common shared-memory parallel-programming primitives. 

Chapter 5 takes an in-depth look at parallelizing one of the simplest problems imaginable, namely counting. Because almost everyone has an excellent grasp of counting, this chapter is able to delve into many important parallel-programming issues without the distractions of more-typical computer-science problems. My impression is that this chapter has seen the greatest use in parallel-programming coursework. 

Chapter 6 introduces a number of design-level methods of addressing the issues identified in Chapter 5. It turns out that it is important to address parallelism at the design level when feasible: To paraphrase Dijkstra, "retrofitted paralleism considered grossly suboptimal". 

The next three chapters examine three important approaches to synchornization. Chapter 7 covers locking, whichi is still not only the workhorse of production-quality parallel programming, but is also widely considered to be parallel programming's worst villain. Chapter 8 gives a brief overview of data ownership, an often overlooked but remarkably pervasive and powerful approach. Finally, Chapter 9 introduces a number of deferred-processing mechanisms, including reference counting, hazard pointers, sequence locking, and RCU. 

Chapter 10 applies the lessons of previous chapters to hash tables, which are heavily used due to their excellent partitionability, which (usually) leads to excellent performance and scalability. 

As many have learned to their sorrow, parallel programming without validation is a sure path to abject failure. Chapter 11 covers various forms of testing. It is of course impossible to test reliability into your program after the fact, so Chapter 12 follows up with a brief overview of a couple of practical approaches to formal verification. 

Chapter 13 contains a series of moderate-sized parallel programming problems. The difficulty of these problems vary, but should be appropriate for someone who has mastered the material in the previous chapters. 

Chapter 14 looks at advanced synchronization methods, including non-blocking synchronization and parallel real-time computing, while Chapter 15 covers the advanced topic of memory ordering. Chapter 16 follows up with some ease-of-use advice. Chapter 17 looks at a few possible future directions, including shared-memory parallel system design, software and hardward transactional memory, and functinal programming for parallelism. Finally, Chapter 18 reviews the material in this book and its origins. 

This chapter is followed by a number of appendices. The most popular of these appears to be Appendix C, which delves even further into memory ordering. Appendix E contains the answers to the infamous Quick Quizzes, which are discussed in the next section. 

