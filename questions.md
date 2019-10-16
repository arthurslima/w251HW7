Describe your solution in detail. What neural network did you use? What dataset was it trained on? What accuracy does it achieve?
  <br>I used the tensorflow lib with a fully-connected neural network trained on the frozen_inference_graph_face dataset. The mean score on the benchmark was of 0.08 
  <br>
Does it achieve reasonable accuracy in your empirical tests? Would you use this solution to develop a robust, production-grade system?
    <br>It performed well on the empirical tests. This solution is a bit less robust then using openCV since it does not have the same frames per second as the openCV
  <br>
What framerate does this method achieve on the Jetson? Where is the bottleneck?
    <br>We were able to run a prediction every 0.3s, making it perform 3 frames per second.
    <br>The bottleneck is the neural net
  <br>
Which is a better quality detector: the OpenCV or yours?
    <br>OpenCV is performing better than my own.
