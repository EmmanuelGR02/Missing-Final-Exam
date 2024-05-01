#	Impact of Missing Final Exam


##	**IMPACT**
### 1. Money
* Retaking the class would require to pay for it once again. A very unfortunate thing for a broke college student (me).
* This might require a loan, which is something I want to avaid as much as possible.
* Spending this money to retake a class could mean that:
	* Canceled planned vacations
	* Less money saved for emergencies
	* Potential failure to make bill payments 
	* Smaller budget for basic needs like, groceries, clothes, gas, etc.

### 2. Time
* In terms of time, it could defenitely delay the year of my graduation, which directly affects the progression in my professional career.
* I would need to keep working two jobs, and ask for more hours to be added into my schedules in order to pay for the tuition. This can affect my time management since I will still be taking other classes, giving me less time to focus on them. More work ours (to pay for the retake) = less time to focus on classes = potential of failing another class = repeat of cycle.

### 3. Professional Life
* Since I mentioned how this event can potentially cause me to fail multiple classes in the worst case senario,
and only one in the best case, it will delay me getting myself out into the professional world. 
It will now take me longer to get into better positions due to aquiring my diplama later than anticipated, 
and I will be less experienced, which is crucial as software companies prioritize experienced candidates.

### 4. Personal Life
* Debt/Less finacially stable
* Less personal time 
* Lots of "what am I doing with my life" thoughts
* All of these impacts will make my parents very upset. (Let's not talk about the lecture my mom gave me
when I told her I didn't wake up for my final)


## **CPE**: `cpe:/h:viviana:emmanuel:21.0`


## **Threat Sources**
### 1. Work:
* Work was definitely a threat source. During the week, I usually go work early morning the days
I didn't have class, and then I went to my other job, which was done at night, and I end the day
by going to the gym. This left me with almost no time to study during the week.
Saturdays and Sundays I only work 4-8 hours early morning, leaving time to study the rest of the day.
### 2. Linear Algebra:
* The final for linear algebra was the main threat source. I had a D on the class, but the professor
said that if we get a 94 on the final, we get a A for the class, or if we get a 85 on the final,
we get a B for the class. I had to go super tryhard on studying 26 chapters. Saturday I 
decided not to pull an all-nighter, so I slept about 4 hours. I called off word Sunday 
so I could study all day and I did pull an all-nighter and did not stop studying until
12:30pm Monday when I had to the final (I got an 85!). After the exam I went to work
and got out at 9, then got home at 9:30 (definitely wasn't going to go to the gym).
I went over the class github for about 2 hours, put 2 alarms and fell asleep. Then I just
woke up at 10, with no memory of me hearing my alarms at all.
* I always hear my alarms (me deciding to snooze 10 times is a different story), but in this case
I don't think putting more than 2 would have made a huge difference. Telling my sibling to wake me
up before she went to school would have been way more effective.
 

## **NIST Standards and Relations #1**
### 1. [Communication Contention](https://cwe.mitre.org/data/definitions/923.html)
* The product establishes a communication channel to (or from) an endpoint for privileged or protected operations, but it does not properly ensure that it is communicating with the correct endpoint.
* This could relate to this event with me setting up my alarms. Due to the lack of sleep and how tired I was, Thers a pretty good chance that I put the alarms for PM instead of AM, but no alarms went off at 7PM. Another possibility is that I somehow just imagined or dreamed that I put my alarms. The event that most makes sense is that I just went to the clock app and looked at my alarms, but didn't really turn on any alarms. I clearly did not properly ensure that the alarms were on, becasue I just can't remember me double checking or hearing them go off in the morning.
### 2. [Resource Depletion](https://cwe.mitre.org/data/definitions/770.html)
* The product allocates a reusable resource or group of resources on behalf of an actor without imposing any restrictions on the size or number of resources that can be allocated, in violation of the intended security policy for that actor.
* In this case, the "resource" is the opportunity to take the final exam. The system (me) failed to properly allocate the resource (time for the exam) due to exhaustion. This led to me missing the final, which is a violation of the intended security policy (ensuring attendance at scheduled exams) and had significant consequences.
### 3. [Mishandling of Critical Information](https://cwe.mitre.org/data/definitions/451.html)
* The user interface (UI) does not properly represent critical information to the user, allowing the information - or its source - to be obscured or spoofed. This is often a component in phishing attacks.
* In this case, the critical information is the date and time of the final exam. The user interface (the alarm clock) failed to properly represent this critical information to the user (me), leading to me missing the final. Possible scenarios:
	* The alarm not clearly displaying the set alarm time.
	* Me failing to clearly differentiate between AM and PM settings.


## **NIST Standards and Relations #2**
### 1. [CWE 693 - Protecting Mechanism Failure](https://cwe.mitre.org/data/definitions/693.html)
* This weakness covers three distinct situations. A "missing" protection mechanism occurs when the application does not define any mechanism against a certain class of attack. An "insufficient" protection mechanism might provide some defenses - for example, against the most common atacks - but it does not protect against everything that is intended. Finally, an "ignored" mechanism occurs when a mechanism is available and in active use whithin the product, but the developer has not applied it in some code path.
* In this event, the "protection mechanism" was my alarm clock being set to wake me up. In terms of the "protection mechanism failures"we have the following:
    * **Missing Mechanism**: `I did not set the alarm at all.`
    * **Insufficient Mechanism**: `The alarms were not enough to wake me up due to my exhaustion.`
    * **Ignored Mechanism**: `The alarm feature on my app works perfectly fine, but I just did not hear the alarms at all and didn't wake up.`
### 2. [CWE 357 - Insufficient UI Warning of Dangerous Operation](https://cwe.mtre.org/data/definitions/357.html)
* The user interface provides a warning to a user regarding dangerous sensitive operations, but the warning is not noticeable enough to warrant attention.
* In this case, the "dangerous sensitive operation" was missing the final exam, and the "user interface" providing a "warning" is my alarms, which were not not noticed by me.

## **Security Policy**
* **Policy**
    * The objective of this policy will be to effectively wake me up so I don't miss an important event.
* **Required resources**
    * Let's say that the problem was that I just didn't hear the alarms. I can fix this by connecting my phone to a speaker and turning it all the way up.
    * I could also manage my time better. In this case I should have started studying for my linear algebra exam earlier, giving me more time to sleep.
* **Implementation**
    * Managing my time in order for me to have time to rest, and also connecting my phone to a speaker so that I can hear my alarms when they go off.
* **Cost**
    * The price of a speaker can vary, but lets say I get one that is $100.
    * Managing my time to have enough time to study for finals could mean that I would need to have less work hours for a week or two, which could reduce my check by about $400.
*   On a side note, about a year an a half ago I wanted to start waking up ealier to be more productive, so I make a "gun alarm" to help me wake up. Using an arduino and a gel bullet gun, I made a program to take an input of how long I wanted to sleep for (a timer) and when the timer hit 0, the gel gun would shoot me for a few seconds, stop, then shoot me again until I stood up to turn it off. It worked. 


## **Conclusion**
* In conclusion the event of me missing a final exam is very crucial to my personal, financial, and professional life.
    * **Personal life**: `Less free time to do things I enjoy due to having to work more hours.`
    * **Professional life**: `Late start to my career.`
    * **Financial life**: `This event could potentially lead into me failing more classes in the future resulting in student debt, and just throwing money away by retaking classes.`
* Although there was a bit of comedy in this assignemt, in a more serious note, I am truly sorry for missing the final exam for your course. At the end of the day there is no excuse. You provided the date and time with plenty of time, and it was my responsaibility to show up. I am very grateful that you gave me the opportunity to pass the class by letting me take the final exam late. Thanks to you, I won't have to go through all of the consequeces talked about in this assignment. Once again, thank you so much, and I hope that my assignment meets your expectations.
        
