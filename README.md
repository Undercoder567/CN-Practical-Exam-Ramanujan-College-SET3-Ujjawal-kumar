# CN-Practical-Exam-Ramanujan-College-SET3-Ujjawal-kumar

**Set-3**

Ujjawal kumar

Sem 3,2nd year

Ramanujan College

College roll no. 20201441

Exam roll no. 20020570038


**CN Practical Exam**

**Ques 1:Simulate and implement go back n sliding window protocol.**

**Explanation**

In computer networks sliding window protocol is a method to transmit data on a network. Sliding window protocol is applied on

the Data Link Layer of OSI model. At data link layer data is in the form of frames. In Networking, Window simply means a

buffer which has data frames that needs to be transmitted.

Both sender and receiver agrees on some window size. If window size=w then after sending w frames sender waits for the

acknowledgement (ack) of the first frame.

As soon as sender receives the acknowledgement of a frame it is replaced by the next frames to be transmitted by the sender. 

If receiver sends a collective or cumulative acknowledgement to sender then it understands that more than one frames are 

properly received, for eg:- if ack of frame 3 is received it understands that frame 1 and frame 2 are received properly.

In sliding window protocol the receiver has to have some memory to compensate any loss in transmission or if the frames are received unordered.

Efficiency of Sliding Window Protocol

η = (W*tx)/(tx+2tp)

W = Window Size

tx = Transmission time

tp = Propagation delay

Sliding window works in full duplex mode

Go back n: Sender transmits all frames present in the window that occurs after the error bit including error bit also.

**Sample output:**
![Ques1  1](https://user-images.githubusercontent.com/83595564/145756508-5228673d-a724-4f0d-bc41-ae7e2f63c5a9.jpg)
![Ques1  2](https://user-images.githubusercontent.com/83595564/145756515-1b45fa13-0e9c-4018-81e4-9a7d359ddd19.jpg)

**-----------------------------------------------------End------------------------_--_-------------------**

**Ques 2:Simulate Cyclic Redundancy Check (CRC) error detection algorithm for noisy channel.**

**Explanation**
