# 5 Things You Should Remember When You Are Getting Code Review

Code review is an essential part of creating high quality software.

One of the things that I disappointed while reviewing co-workers code at work a few years ago was the attitude. In a code review conducted with several people, if one of them speaks emotionally, the person who is receiving the review is likely to be tired and upset. No matter how code review to make better software, but who would like it if they heard sadistic words when they did their best?

So I'm going to summarize the 5 things that I think would be fine if we knew each other.

---

## 1. Avoid Aggressive Questions

> "Why did you write it like this?"

This kind of question makes the listener feel uncomfortable. And it embarrasses people who are watching the code review. Remember the purpose of code review. We are doing this not to criticize other people's code and/or to imprint that who is more superior but to find bugs in advance and make better software.

> "How about this one?"

Let's start to talk like this. However, we should make it clear that it is not a personal taste by giving a proper explanation or reason.

---

## 2. Listen First and Speak Last

If the reviewer keeps making comments while he/she is explaining the code and intention, the flow will break repeatedly. And not only who are receiving code review but also those who are watching the code review are getting tired. Taking notes or remembering rather than immediately discussing improvements or questions about code is much more effective at avoiding emotional comments. Because it makes you think again.

At this moment, the person who wrote the code will need the trick of cutting it off properly so that it will not be taken too long like in terms of class file or small business unit.

---

## 3. Praise and Encourage Immediately

> "I think this code is very good."

> "Looking at the code you wrote, you must have had a hard time..."

What more needs to be said?

---

## 4. Avoid Unnecessary Arguments

There is no worse code review than discussing "Declaring variables across multiple lines v.s. Declaring variables side-by-side with commas". Of course, that wasn't the main issue of the code review but let's respect other people's tastes. Nevertheless, if it is bothering you, defining code conventions after gaining majority consent can be a good way to avoid unnecessary arguments.

---

## 5. Give Direction for Good Code, but Don’t Force It

> "You have to change this line like this."

Is it an industry standard? Then accept it. Is it a ground rule on your team? Accept it too. Is there a potential possibility of an error if you don't change it? Fix it right away.

What I mean is don't force changes to code that works regardless of the changes. If it is not a violation of an industry standard or ground rule, then it should be their choice whether to change it or not. If the reviewer forces such a code so that members receives a negative result such as **Failed** or **Rejected**, then the team members will blame themselves. Furthermore, the morale of the entire team will drop at some point. These threats should be eliminated whenever possible.