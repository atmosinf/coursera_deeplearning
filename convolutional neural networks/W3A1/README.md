## Screenshots from the lectures<br>

![1](screenshots/1.PNG)<br><br>
![2](screenshots/2.PNG)<br><br>
![3](screenshots/3.PNG)<br><br>
**You can use a log likelihood loss for C1, C2 and C3. For the bounding box outputs you can use squared error or something like squared error. For Pc you can use a logistic regression loss**
![4](screenshots/4.PNG)<br><br>
**The identity of the landmark points must be consistent across different images. For instance l1x,l1y is the left corner of the left eye (when looking at the image)**
![5](screenshots/5.PNG)<br><br>
**The training set is closely cropped - the car takes up all of the image without much background**<br>
![6](screenshots/6.PNG)<br><br>
**The sliding windows method is computationally costly. Small strides require more computation, while larger have poorer performance**<br>
![7](screenshots/7.PNG)<br><br>
![8](screenshots/8.PNG)<br><br>
![9](screenshots/9.PNG)<br><br>
![10](screenshots/10.PNG)<br><br>
![11](screenshots/11.PNG)<br><br>
![12](screenshots/12.PNG)<br><br>
![13](screenshots/13.PNG)<br><br>
**What non-max suppression does, is it cleans up these detections. So they end up with just one detection per car, rather than multiple detections per car**<br>
![14](screenshots/14.PNG)<br><br>
![15](screenshots/15.PNG)<br><br>
![16](screenshots/16.PNG)<br><br>
![17](screenshots/17.PNG)<br><br>
**Now, just some additional details. What if you have two anchor boxes but three objects in the same grid cell? That's one case that this algorithm doesn't handle well. Hopefully, it won't happen. But if it does, this algorithm doesn't have a great way of handling it. I will just influence some default tiebreaker for that case. Or what if you have two objects associated with the same grid cell, but both of them have the same anchor box shape? Again, that's another case that this algorithm doesn't handle well. If you influence some default way of tiebreaking if that happens, hopefully this won't happen with your data set, it won't happen much at all. And so, it shouldn't affect performance as much.**<br>
![18](screenshots/18.PNG)<br><br>
**Oh and as usual for simplicity on the slide I've used a 3 by 3 the grid. In practice it might be more like a 19 by 19 by 16. Or in fact if you use more anchor boxes, maybe 19 by 19 by 5 x 8 because five times eight is 40. So it will be 19 by 19 by 40. That's if you use five anchor boxes. So that's training and you train ConvNet that inputs an image, maybe 100 by 100 by 3, and your ConvNet would then finally output this output volume in our example, 3 by 3 by 16 or 3 by 3 by 2 by 8**<br>
![19](screenshots/19.PNG)<br><br>
![20](screenshots/20.PNG)<br><br>
![21](screenshots/21.PNG)<br><br>
![22](screenshots/22.PNG)<br><br>
![23](screenshots/23.PNG)<br><br>
![24](screenshots/24.PNG)<br><br>
**So the idea of region proposals has been quite influential in computer vision, and I wanted you to know about these ideas because you see others still used these ideas, for myself, and this is my personal opinion, not the opinion of the computer vision research committee as a whole. I think that we can propose an interesting idea but that not having two steps, first, proposed region and then crossfire, being able to do everything more or at the same time, similar to the YOLO or the You Only Look Once algorithm that seems to me like a more promising direction for the long term. But that's my personal opinion and not necessary the opinion of the whole computer vision research committee.**<br>
![25](screenshots/25.PNG)<br><br>
![26](screenshots/26.PNG)<br><br>
![27](screenshots/27.PNG)<br><br>
![28](screenshots/28.PNG)<br><br>
![29](screenshots/29.PNG)<br><br>
![30](screenshots/30.PNG)<br><br>
![31](screenshots/31.PNG)<br><br>
![32](screenshots/32.PNG)<br><br>
**In case you're wondering why do we have to do it this way, I think there are multiple possible ways to take small inputs and turn it into bigger outputs, but the transpose convolution happens to be one that is effective and when you learn all the parameters of the filter here, this turns out to give good results when you put this in the context of the union which is the learning algorithm will use now.**<br>
![33](screenshots/33.PNG)<br><br>
![34](screenshots/34.PNG)<br><br>
![35](screenshots/35.PNG)<br><br>

## Quiz <br>

![q1](screenshots/q1.PNG)<br><br>
![q2](screenshots/q2.PNG)<br><br>
![q3](screenshots/q3.PNG)<br><br>
![q4](screenshots/q4.PNG)<br><br>
![q5](screenshots/q5.PNG)<br><br>
![q6](screenshots/q6.PNG)<br><br>
![q7](screenshots/q7.PNG)<br><br>
![q8](screenshots/q8.PNG)<br><br>