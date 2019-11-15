# Video-Steganography
Secure transmission of image/text by using video as a "cover"


Steganography is the art and science of sending covert messages such that the existence and nature of such a message is only known by the sender and intended recipient.
It involves concealing a file, message, image, or video within another file, message, image, or video. If cover is video file then it is called Video Steganography.

Objective: To design A Highly Secure Video Steganography using Hamming Code (7, 4)

At sender's side:
1.Conversion of video frames into a YUV format.
2.Applying (7, 4) Hamming code to 1D structure of message which is a image to obtain the codeword.
3.Embedding the message codeword into the video frames.
4.Reconstruct the video from the frames.

Receiver’s side:
1.Split the received video into frames and convert them to YUV format.
2.Retrieve back the message codeword from the frames.
3.Retrieve back original message from the message codeword by using decoding for hamming code.

Algorithm:
The algorithm requires a video to be converted into frames and changing the pixel positions. 
The message which is to be transmitted must be converted into one-dimension, XOR and Hamming code are applied to this message. 
Then this encoded message is embedded in the scrambled video frames. These frames are reconstructed and sent to the receiver. 
The receiver can extract information using the same key as the sender side. 
The receiver has to disassemble the video, use XOR and hamming code to reconstruct the correct intended message.



Working with the files:
Run the file in the following order: m1.m ,m2.m, m3.m, m4.m, m5.m, m6.m
