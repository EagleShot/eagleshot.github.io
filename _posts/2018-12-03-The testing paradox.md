---
layout: post
title: The testing paradox
tags: ["Senior Seminar","Software Engineering"]
excerpt: "Even though testing of software code is essential, even tested code does not gaurantee that it will always work. So what's the value in testing?"
comments: true
---

If you have ever completed a programming course, you will probably have heard this a thousand times: "Always test your code" or "Code a little, test a little." Code that is not tested cannot be considered complete because its validity has not been checked. So when sufficient tests are written for a piece of code, one might come to believe that the software is correct and free of bugs. This is a fallacy of software development: Testing only shows the presence of defects. It does not prove that it is free of them.

A test can only detect errors that the programmer has accounted for. This can be avoided by brute force testing of all the input space, but for any real-life software, this is infeasible because of the input space. Every programmer wants their code to be error free. Certain kinds of software like mission-critical software (power grid, airplane, nuclear reactors) and medical applications do not have any margin of error, and when mistakes do exist, it can cause loss of life. Then how does one know when test have sufficiently tested?

This comes from practice and experience. Testing can also be done as a black box which in which the tester does not have access to the code. This helps to prevent bias, but as the tester does not have access to the code, they can be wasting a lot of time testing for cases that have clearly been covered. Then there is white box testing which is the other extreme where the tester not only has access to the code but also have the ability to change the code and execute the modified version. This helps to see behavior that is different from the provided source code and test for edge cases that the code necessarily does not allow. The middle ground between the two is called grey box testing and allows the tester access to the source but does not allow for modification. This helps to prevent a waste of time while maintaining the coding responsibilities and preventing testers from modifying the source.

There is a whole branch of computer science that deals with proving the correctness of a piece of software. It uses techniques of automatic theorem proving to check the program. There have been advances made in this field, and there is software that helps to determine the correctness of the program, but they only work for small to medium-sized applications. Until there is significant progress in the field, good software practice and careful testing is the way.
