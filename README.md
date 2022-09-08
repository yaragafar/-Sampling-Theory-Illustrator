# Sampling-Theory-Illustrator
A digital signal processing desktop app using python and PyQt5 where users choose a signal, its sampling rate, and can reconstruct it based on The Nyquist–Shannon sampling theorem.

## Team members
- Yara Hossam
- Haidy Sayed
- Hagar Ashraf
- Hussien Rashidy

## Introduction
Sampling an analog signal is a crucial step for any digital signal processing system. The Nyquist–Shannon 
sampling theorem guarantees a full recovery of the signal when sampling with a frequency larger than or equal to the 
bandwidth of the signal (or double the maximum frequency in case of real signals).

## Tools
- Python
-PyQt5
-QtDesigner

## Description
An illustrator for the signal recovery that shows the importance and validation of the Nyquist rate.
- The application allows the user to open a mid-length signal (around 1000 points length) and show it on 
the main graph.
- The user can sample the given/read signal and see the sampled points highlighted on top of the signal.
- The user can change the sampling rate via a slider that range from 0 Hz to 3fmax, where fmax is the maximum 
frequency in the read signal. When changing the sampling frequency, the sampled points are expected to be 
changed on the graph (ofcourse, the original signal will encounter no change when changing the sample rate).
- The app is able to reconstruct/recover the signal from the sampled points. 
- The user is able to see the reconstructed signal from the sampled points as a new signal in a secondary graph below the main graph.
- The user can toggle the visibility of the secondary graph via some UI element (button or menu item) such that 
when it disappears, the main graph takes the whole space of the app window.
- The user is able to maximize the app window. i.e., when maximized, all your control should 
resize/rescale to fill the window properly.


- The application provides the user with a primitive signal composer where s/he can generate basic signals 
to test and validate on the app. Each signal is basically a summation of some sinusoidals and each sinusoidal has 
a specific frequency, magnitude and phase shift. The Signal Composer shows up as a separate tab in the 
application. The Composer has the following functionalities:
1) One graph to display the sinusoidal to be generated. A small panel shows beside the graph to 
control the frequency, magnitude and phase of the sinusoidal. Then, a button to confirm and add this 
sinusoidal to the summation.
2) One graph to display the sum of the generated sinusoidals. There is a combobox 
through which the user can select one of the contributing sinusoidals and remove it via a delete button.
3) When the user is settled on his/her synthetic signal (the one that shows up in the second graph), s/he 
confirm moving it to the main illustrator graph to start the sampling/recovery process.

## Demo

### Composer

1) One graph to display the sinusoidal to be generated. A small panel shows beside the graph to 
control the frequency, magnitude and phase of the sinusoidal. Then, a button to confirm and add this 
sinusoidal to the summation.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/draw_signal.gif)

2) One graph to display the sum of the generated sinusoidals. 
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/sum_compose.gif)

There is a combobox through which the user can select one of the contributing sinusoidals and remove it via a delete button.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/remove.gif)

3) When the user is settled on his/her synthetic signal (the one that shows up in the second graph), s/he 
confirm moving it to the main illustrator graph to start the sampling/recovery process.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/save.gif)

![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/move_to_main.gif)

### sampling
- The application allows the user to open a mid-length signal (around 1000 points length) and show it on 
the main graph.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/open_file.gif)

- The user can sample the given/read signal and see the sampled points highlighted on top of the signal.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/sampling.png)

- The user can change the sampling rate via a slider that range from 0 Hz to 3fmax, where fmax is the maximum 
frequency in the read signal. When changing the sampling frequency, the sampled points are expected to be 
changed on the graph (ofcourse, the original signal will encounter no change when changing the sample rate).
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/sampling2.png)

- The app is able to reconstruct/recover the signal from the sampled points. 
- The user is able to see the reconstructed signal from the sampled points as a new signal in a secondary graph below the main graph.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/reconstruct.png)

- The user can toggle the visibility of the secondary graph via some UI element (button or menu item) such that 
when it disappears, the main graph takes the whole space of the app window.
![](https://github.com/yaragafar/Sampling-Theory-Illustrator/blob/main/gifs/show_hide.gif)
