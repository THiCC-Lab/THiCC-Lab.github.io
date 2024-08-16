---
layout: post
title:  "Meera Ray and Her Research With AI-SDM"
author: meera
categories: [ Interviews, AI-SDM ]
image: https://images.unsplash.com/photo-1454789476662-53eb23ba5907?q=80&w=3452&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

Sage:
What is the official title of your research project?

Meera:
The title of our project is “Vector Symbolic Decision-Making Models for Disaster Recovery”.

Sage:
Can you summarize the main objectives of your research?

Meera:
Yes, we want to model how people who are surviving a natural disaster respond to them, their circumstances, how they go to shelters, and how they acquire resources that they need to survive and recover from a disaster, which means returning to their original state before it happened. My specific project is a cognitive model. Cognitive models are like processes in the mind when people make decisions and their vector symbolic because it assigns each symbol in memory, each concept, a large vector of numbers. These vectors represent the relationships of these concepts to each other.

Sage:
You are modeling natural disaster responses, seeing how systems allocate resources for their response, and then modeling the human mind with what you said are vectors, but they are just computations, right?

Meera:
It is a computational model. Primarily because we are trying to model people surviving a natural disaster. The people we would give this give this to are the decision makers, the emergency managers.

Sage:
Can you describe the methodology you use in your research? More specifically, the simulation steps?


Meera:
Yeah. Right now, we are still in the stage of developing the inner workings, the mechanics of the model. We have not gotten to actual human subjects yet. For example, how do you encode a certain piece of memory? You get an input from the environment and your brain needs to have some sort of representation? You could call it an engram; I believe that is what it is called in cognitive science. What is the computational representation of that? That is what we must figure out. I have been using something called holographic declarative memory. It represents chunks of memory as vectors that are bound together and stored in a vector space. What I have been doing is making HDM (Holographic Declarative Memory) work ACT-R (Adaptive Controlled Thought-Rationale). ACT-R is a cognitive architecture. It comes from rational analysis, like Bayesian methods. You have a prior belief about something, you have evidence, you update it to the posterior. It inspired some of the equations behind how ACT-R works. It is a basic framework for how the mind works. It has modules for memory, which procedures you would take, long term memory, and short-term working memory.

Sage:
You said HDM works with ACT-R?

Meera:
HDM works with ACT-R. Most of my work so far has been getting HDM to work with ACT-R correctly.

Sage:
What are the advantages and limitations of the methods you used?

Meera:
Some of the advantages is that ACT-R is a very old, well developed cognitive architecture. There is plenty of documentation and examples of it out there. A disadvantage is that the main popular version of ACT-R is written in Lisp. A language if I remember correctly, that has been around since the 1970s. I had to learn how to work with it correctly.

Sage:
What is the main language of HDM?

Meera:
HDM was specified as a concept. There is Python code out there, but it was not complete for working with the main version of ACT-R. It is in Python, and I have been developing it in Python.
Sage:
Would you say you have been learning how to make Lisp to work with modern Python?

Meera:
There has been a lot of bridging. Deja has also been working with that. It has been a challenge for both of us.

Sage:
What, if any, key findings have you found so far?

Meera:
Yeah, we are still initial, I started working on this in the fall. We want HDM to be able to recall an entire chunk of memory. In cognitive science terms, a chunk is bits of memory that are grouped together, so that they've effectively function as one memory. For example, people tend to have a hard time remembering 15 individual letters but if those 15 letters are two words, then it is easy. We want to be able to recall an entire chunk of memory, given just a certain part of it. For example, you might know someone's name and then you can explain where they are from, who their friends are, and all the associated memories about them. HDM doesn't by itself, do that. That was not even theoretically specified. I have been coming up with a theory for how to do that, the math behind it, and coding it up. 
My initial findings are that we can represent chunks of memory that are entered into HDM as you a temporal encoding. All these bits of memory are entered at the same time, then we want to represent that time as a vector that is associated with each of the bits of memory. We found it is very preliminary, but neural oscillator encodings have been relatively successful at distinguishing which bits of memory are chunked together. I am not a cognitive science person. In undergraduate, I studied statistics and machine learning. That is the kind of AI people think of when they hear AI these days. It is a very applied statistics for numerical optimization. I didn't know anything about cognitive science. And at first, I didn't really get how it was related. AI at the very beginning was like, we want systems that are adaptive, able to learn, and make autonomous decisions. What examples do we already have of this? Well, a person. That is what a person's brain does. If we can understand how their brain works and understand how the mind makes decisions, then we can get some insights from there. AI these days has drifted away from that. The old cognitive science roots of AI are still around. That is what ACT-R people are doing. That is why I ended up having to read about, what are some ways the brain encodes temporal information? How do you distinguish 3:30pm from 4pm or from 4:30pm? One answer is oscillators (sine or cosine functions). The idea is that you would have a bunch of different oscillators together, some of them have a high frequency, some low. You would be able to take a value at a certain point of each oscillator and then you end up with an entire vector for each timeframe. You want there to be a full similarity between one time vector and another time vector if they are from the same time and different if they are from different times. With cognitive science-based AI, you actually want it to make mistakes. You want it to make the same kind of mistakes a person would. You will notice that if you are trying to remember a time and guessed incorrectly, you are more likely to guess a time that is on the same hierarchy. For example, if you are trying to remember that a certain event happened at 3:30pm, you are more willing to mix that up with 4:30pm than 4:15pm because they have the same seconds value. That is why that there should be some error.  Not a global maximum, but a bunch of local maxima to accurately represent the errors a person would make.

Sage:
What would the simulation look like? What would the simulation do?

Meera:
It is supposed to ask people a series of questions and they will make certain choices. Some of the choices would be different directions for navigating through a maze called a minimap, trying to figure out which places are the best for you to go with a limited number of moves. This is not the same as measuring people in a disaster but there are strong ethical reasons for that. “Hey, I know you and your family are escaping from a flood, but can you be in our study right now?” Yeah, we do not want to do that. Once this model is more developed, we want to get human subjects to play this simulation game so we can analyze what decisions they make. Then my model will also do the simulation and we will be able to see what discrepancies exist. How well are we able to predict their behavior? How well can we model it? My model would be entered into the same game environment as the human participants. It would interact with the environment, get inputs from the environment, take a certain action, and make a certain decision to take an action. We would have human and non-human players. and we would want to see if we can make the model effectively represent actual human decision-making processes.

Sage:
Would the agent and human competitors be competing at the same time?

Meera:
Right now, they would not. We would just get the data from the humans and see if I can make a model that matches their data correctly? That is a research goal. I cannot tell you if we will get there. We will most certainly try.

Sage:
Anything about the research process so far that surprised you?

Meera:
I was not expecting to have to deeply understand cognition and what are some biologically plausible ways that people remember certain things and associate memories together? That is not my background originally. I thought it would just be like a programming problem, like connecting these two systems together. It ended up being more than that. I had to get involved with a lot more cognitive science.

Sage:
How did you ensure the validity of your findings?

Meera:
We have not gotten there yet. The future concern I have is that there is a physiological problem, where you want to have a hypothesis that is declared at the beginning before we start the scientific process. Otherwise, you can make spontaneous conclusions. For example, if I do not know what a model is going to look like at all and I see the human data and then a build a model off that, then I have something circular. That is something I want to avoid. I want to make sure my model is somewhat well developed before I look at human data.

Sage:
Is there any possibility of cheating during the game?

Meera:
I do not think so. We are not at that stage yet but that is something we would look out for in the future.

Sage:
What are the main challenges you have encountered during your research?

Meera:
Sometimes it is not clear about the rationale behind why programmers made a certain decision with code, especially for small academic projects. You must spend more learning the code and figuring out how the different parts fit together.


Sage:
This project is working with AI-SDM (AI Institute for Societal Decision Making). How does this research contribute to their overall goal?

Meera:
One of AI-SDM’s use cases is disaster management, like response and recovery. The idea is that we can go to an emergency manager, the person who is tasked with organizing and coordinating your response to a natural disaster in their jurisdiction. When they decide about where to put resource centers or shelters, we can give them the simulation so they can see what kind of decisions people in a certain area, depending on their distance from a shelter, their social background, and what resources they have access to, would make. This gives emergency managers extra aid to better make decisions. They are overwhelmed with information, and they must make a series of decisions that put a lot of strain on the human mind. We only have so much cognitive capacity, right?

Sage:
Are there any interdisciplinary aspects that have been crucial to your work? I imagine cognitive science with computer science is a big part. 

Meera:
Yeah, definitely. 

Sage:
How does your research fit into the bigger picture of research in your field?

Meera:
In the overall AI field, there has been a move away from cognitive science. The projects that get the most funding, both in academic departments and in the industry, have been more tailored towards narrower goals of improving performance and efficiency, like neural networks. You will notice that they are inspired by the brain, there's activations and connections but the actual ways they are trained, and the way they are structured is become just increasingly unmoored from anything that would happen in our brain. There are different research methods and I think we could benefit from a diversity of them. I believe there is value to understanding how the mind works and using those insights when we build our own AI systems. I like to think my work makes a small push back to the roots of cognitive science and psychology.

Sage:
Are there any other potential applications for this research?

Meera:
Yeah, as climate change goes on, there are going to be more natural disasters and their severity and frequency are increasing. The amount of people they will have an impact on will increase. Unless we invest in these kinds of resources to allocate everything efficiently, a lot of people are going to be harmed. There is a well-known inequality about how people are impacted by disasters. If you were already in a disadvantaged social situation before the disaster, you are going to be even more disadvantaged after it. There are historic and ongoing examples of disaster responders, people who work in disaster recovery, making decisions about which communities to put resources into that consistently serve those who already were better off, like Hurricane Katrina. The response was an infamous example of this. In New Orleans, when white neighborhoods received aid faster, there was a perception that the flooding had stopped in those communities first. This is something that has gone on in various forms and lots of disasters. We are in the US context. I can only speak to that, but I am sure in other places, too. That is something we explicitly want to address. That is what this work is about. 

Sage:
For this project the focus is on U.S. interests, but do plan on eventually expanding internationally?

Meera:
I do not see why our framework could not be used in other places, but AI-SDM’s funding is from the National Science Foundation. We are mostly only talking with emergency managers in Pennsylvania, so right now, no. It is very important for us to talk to the people that this tool will be going to. We do not want to make these systems while being disconnected from the reality of who would use them. We want to meet their needs.

Sage:
Are there any ethical considerations or implications associated with your research?

Meera:	
If you are going to be creating something that influences decision makers, well real people will be affected and that is something you have to think about, how the tool functions. We need to be very transparent about what data we are putting into the model. Dataset transparency is a big issue right now, especially with large language models. For example, Open AI’s Chat GTP systems have not disclosed what data they have used and how it was processed. That is something we want to be as transparent about as possible.

Sage:
What is the future for this project?

Meera:
Right now, we are still at the initial stages. I want to get the model to recall an entire chunk at once. In ACT-R, when you create a model, the modeler needs to manually create the rules. The procedures are if-then rules. If you receive some input from your environment, then carry out this action, which could be recalling a memory or taking an action on the environment. First, I want to finish the HDM backend. Which means full chink recall working fully with ACT-R. We are relatively close to that. I do not want to speak too soon, but I think by the end of the summer, that should be done. Then we want to connect this ACT-R-HDM model with the simulation. We plan to work with Cody Gonzalez’s research, Instance-based Learning (IBL). It is a specification of a cognitive model that continually improves its decisions through iterated decision making. It works by seeing an environment and then selecting an instance that is most like what it is now and takes an action that it remembers being successful. She successfully modeled other types of human decision making before this way. It is based on ACT-R, but it is heavily modified. We believe the HDM-based actor will work better with IBL.

Sage:
Is Dr. Gonzalez’s simulation more representative of a disaster situation? 

Meera:
I believe that one simulation that she worked on was a firefighter rescue simulation. The application you set up is up to you. You design how the map looks, how the points work, and what decisions they take. Our overall goal is that we get all the systems connected, we start getting human subjects, gathering data, and then see if we can model it correctly.

Sage:
Okay, how did you get started in this area of research?



Meera:
I just finished my first year as a PhD student. I joined last August. I did my undergraduate at Carnegie Mellon University with a Statistics and Machine Learning major. It is a subfield of AI, but it is the kind of AI that is more concerned with having a dataset and building a statistical model that maximizes the likelihood of that data. There are valuable principles I learned that I am still going to take into this project, but it was not cognitive science-based at all. I had a personal interest in studying social systems and social reproduction. Why is it that society is arranged the way it is? Why is it that it continues to be arranged that way? What are the processes that create that arrangement? It is social theory. I had a personal interest in that, I did some classes in it, but it was not my major. I did not think there any lab that worked both on things like AI and social theory. I had no idea that anyone was doing that kind of work. When I applied for PhD programs, including at Penn State, Dr. Dancy reached out to me. I checked out the Lab website and was very impressed. I did not have any idea that there were people who were working on both of them.

Sage:
What aspects do you find most exciting about your work?

Meera:
A lot of this is new. ACT-R by itself is relatively old. What's exciting is that we have these relatively old systems that have been around a long time, but we are coming in with newer technology from machine learning like putting an entire body of text into the knowledge of a cognitive model. That is what language models do. It feels like we are like breathing new life into something old. HDMs are a relatively new system that has not been fully connected with the version of ACT-R that is most widely used by researchers. It has not been fully taken advantage of yet. Even beyond this project, if we want to make the code public, then other ACT-R researchers worldwide will get to use our code to build their own models. It is like a larger contribution. What I am working on with HDM, the time encodings and incorporating that into the cognitive model. As far as I have seen, no one has done that yet, which means it is challenging and not guaranteed to work. But that is the fun of research, right?

Sage:
How did your perspective on this topic evolve throughout the course of your, I guess, development stage?

Meera:
I saw this more as a software engineering problem. I got an older system and a newer system, some code that has been written, but I need to expand it. I am used to thinking from more of an engineering perspective about problems, but through meetings with Dr. Dancy and readings I have done for the lab, I started to think about it more as a cognition problem, like what is the extent that we can model the way our brains work?

Sage:
What are the biggest personal lessons you have learned during the research process?

Meera:
I learned to not be intimidated by a new field. You might not understand the new terms, maybe you aren't familiar with the author's or the kind of work they are doing. I know when pretty much anyone reads a paper, sometimes it is like, “Oh my God, I do not understand who they are referencing. I do not understand the context for anything they are talking about.” You can read a paper and read other papers in the field and work with it yourself and slowly enough, you will begin to understand what is important.

---
