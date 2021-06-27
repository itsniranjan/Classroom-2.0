# C L A S S R O O M  2.0



##🤔 A ubiquitous problem

_‘Around 60% of college students in the state have experienced mental depression in varying degrees since the outbreak of Covid-19 and at least 55% of youngsters pursuing UG and PG courses in arts and science colleges are too worried about their future.’_ - Times Of India

<img src="https://static.toiimg.com/thumb/msid-76456212,width-1200,height-900,resizemode-4/.jpg" alt="drawing" width="500" /> 
We broadcasted a survey regarding the mentality of students towards online classes and the results were too disappointing to be true. 90% of students said they would join the classroom and then be involved in their activities or rather sleep. All of them wanted their offline mode of classroom so badly and missed the chit chats and jokes they shared with their benchmates while in class. This created tensions for the teachers as well as they weren’t satisfied about the students easily copying during examinations and the negligence to studies spreading among students
The essentiality to recreate the good old days and make teachers ensure that students were really learning motivated us to create a ‘newer’ normal to education - Classroom 2.0

##⚡ A unique solution

We reimagined the classroom world in the virtual platform by creating a desktop app that covers all the problems faced by teachers as well as students. An app where students can experience an offline classroom, do little chit chats with their benchmates (with time limits), where teachers can ensure that students aren’t switching tabs on their device during the class, where tests can be conducted by leaving no room for cheating in forms of copying from other sources etc. Classes will be fruitful only if both the students and teachers are at comfort. Hence arose our solution incorporating both sides of the medium.

<!--
![image](https://user-images.githubusercontent.com/65534301/123528489-04c8aa00-d705-11eb-99a0-1a8f8236aabf.png) -->
<img src="https://user-images.githubusercontent.com/65534301/123528489-04c8aa00-d705-11eb-99a0-1a8f8236aabf.png" alt="drawing" width="500" />
<img src="https://user-images.githubusercontent.com/65534301/123528524-7acd1100-d705-11eb-80fe-2d4fc91f0d96.png" alt="drawing" width="500" />
<img src="https://user-images.githubusercontent.com/65534301/123528534-a0f2b100-d705-11eb-9a63-507d4c363725.png" alt="drawing" width="500" />
<img src="https://user-images.githubusercontent.com/65534301/123528547-b1a32700-d705-11eb-93eb-a10bd7e4517b.png" alt="drawing" width="500" />
<img src="https://user-images.githubusercontent.com/65534301/123528556-c089d980-d705-11eb-8986-78c3c2d34924.png" alt="drawing" width="500" />

##💻 Implementation

Now more about the implementation of the software. As we are having a demand for separate logins for both teacher and student in the same place, we are using Firebase for its excellent authorization functions and easy to use SDK. We are providing the option to either login via Email or Google. The user auth data is stored in Firestore so that we can also integrate the user role i.e. whether the teacher is Teacher or Student. In the client app as we are using React.js, we can apply conditional rendering depending on the user role, so that both teacher and student get separate layouts. The video call is facilitated by WebRTC - a free open source project providing Real Time Communication (RTC). The SDP protocols are stored in a different Firestore Collection. This will be implemented for a teacher and the connection request is also sent to Firestore for validation and data can be transmitted between the users. To implement a voice channel between benchmates we can also spin up a SDP connection when the seats are chosen, and the data is monitored. If it exceeds a threshold then a request is sent to the teacher via a cloud function. The teacher can disable the frame of the desktop app and make it full screen and the on screen time is recorded for the attendance and a .csv file with the data is generated and shared with the teacher.

##🤝 Redefining meetings

> Teachers can ensure the presence of students in their class via the full screen lock feature of the application.
>
> Students no longer have to attend their classes “alone” and can easily communicate with their classmates to get rid of the black screen monotony
>
> Teachers now have the option to display pop up questions in order to check the student activity status.
>
> Enhanced voice channels to avoid disruptions
>
> Teachers do not have to keep track of attendance since the log will be shown after each class
>
> Teachers have complete control over the voice channels of students in case of ruckus.
>
> Live instant reactions can be given by students about the class ,creating a gripping room for the teachers.
>
> Students can choose their “Benches” as they would in a normal classroom
>
> Students now have a permanent link to their one classroom in contrast to the present method where each subject has a different link.
>
> Gives the feel of an offline classroom virtually.

##😀 Challenges we ran into

> Poor network connection resulting in meeting hold ups.
>
> Initially, most of the team members were unfamiliar with the technologies used.
>
> We ran into a lot of bugs which ate up a huge chunk of our time.

##😍 Accomplishments We're Proud Of:

- As students we always wanted to do something to make this dull online way of learning interactive. So, the successful implementation of this idea itself is a proud manoeuvre.
- Moreover, what makes us more excited is that we were able to complete a major part of this in such a short span of time.
- Encouragements from our teachers as well as students. They just can't wait to see this product in deployment

## 🤓 What We Learned

We could learn a lot in such a short time. We were able to learn new technologies like figma, firebase, WebRTC, Electron in depth. The experience of working remotely as a team was something new to us and gave us a lot of insights. It was a great experience and we could learn to manage our time. Even in middle of college works and personal responsibilities, we managed to find time and had several late night meet-ups.

## 🔥 What next?

- Features such as ML face detection so that it can analyze if the students are concentrating in the class and accordingly mark the attendance
- Examination mode with face detection and disabled voice channels so that exams can be held in a rightful and efficient way.
- We are also planning to include a feature that shows the network connectivity status of each student.
- An alerting system that alerts teachers to give a break to students from extended screen times.

## ⚙ Built with

- [x] Electron
- [x] ReactJS
- [x] Firebase
- [x] Typescript
- [x] Figma
- [x] webRTC

## 👬 👨🏽‍🤝‍👨🏻 Team Members

1. [Goutham Byju](https://github.com/geebee49)
2. [Abil Savio](https://github.com/ByteCrak07)
3. [Niranjan Neelakantan](https://github.com/itsniranjan)
4. [Navneeth Variar](https://github.com/navneethvariar14)
