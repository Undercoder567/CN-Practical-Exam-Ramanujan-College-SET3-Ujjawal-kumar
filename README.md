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

In computer networks sliding window protocol is a method to transmit data on a network. Sliding window protocol is applied on the Data Link Layer of OSI model. At data link layer data is in the form of frames. In Networking, Window simply means a buffer which has data frames that needs to be transmitted.

Both sender and receiver agrees on some window size. If window size=w then after sending w frames sender waits for the acknowledgement (ack) of the first frame.

As soon as sender receives the acknowledgement of a frame it is replaced by the next frames to be transmitted by the sender. If receiver sends a collective or cumulative acknowledgement to sender then it understands that more than one frames are properly received, for eg:- if ack of frame 3 is received it understands that frame 1 and frame 2 are received properly.



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

**Cyclic Redundancy Check and Modulous-2 Division**

CRC or Cyclic Redundancy Check is a method of detecting accidental changes/errors in the communication channel. 
CRC uses Generator Polynomial which is available on both sender and receiver side.

n : Number of bits in data to be sent 
    from sender side.  
k : Number of bits in the key obtained 
    from generator polynomial.
   
   **Sender Side (Generation of Encoded Data from Data and Generator Polynomial (or Key)): **
   
  1.The binary data is first augmented by adding k-1 zeros in the end of the data

  2.Use modulo-2 binary division to divide binary data by the key and store remainder of division.

  3.Append the remainder at the end of the data to form the encoded data and send the same
  
 **Receiver Side (Check if there are errors introduced in transmission)**

**Perform modulo-2 division again and if the remainder is 0, then there are no errors.**
 for eg. we have sent data 10110 through sender end and the receiver received same data 10110 then their is no problem in transmission of data and the operation was successful. 
 
 **Sample output**
 ![Ques2](https://user-images.githubusercontent.com/83595564/145758142-2ef55c54-37d5-4ce5-b884-08bd46919e96.jpg)

