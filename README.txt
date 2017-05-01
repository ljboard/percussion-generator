Elizabeth Board
ejboard
Project 5: Real-Time Performance

For my final project, I created a drum accompaniment pattern. I algorithmically generated patterns using Markov chains, where the states were the beat number (including quarter, eighth, sixteenth, and triplets). The models were trained on drum sheet music samples that included low, middle, and high percussion types. During the concert, the program followed the Markov chains, as well as the current bpm/bps to generate rhythm patterns.

In my interim report, I planned to train the model to select the best instrument for each beat, but Professor Dannenberg suggested that I train a different model on each instrument (rather than one that also selects an instrument). So, I trained 3 models: one for low (e.g. bass) beats, one for mid (e.g. snare/tom) beats, and one for high (e.g. high hat/crash cymbals) beats. Then the three instruments would play independently and can on the same beats, creating a more realistic drum sound. 

I also implemented manual controls that allowed for some real-time input during the concert: optional looping (and choosing the number of measures in the loop), adding pauses (skipping a beat, either none, a selected beat, or a random beat), and volumes (controls for each of the three instruments).

--

Copy of the interim report: 

I will be working on Project 5 alone. I plan to create a drum accompaniment pattern. I will algorithmically generate patterns using a Markov chain (where the state is the beat number, including both on- and off-beats), trained on audio samples in different genres (then during the concert, the program will use the current genre, bpm, and bps to select which pattern to follow). The patterns will also be trained to select the ‘best’ instrument (bass, snare, hi hat, cymbals) for each beat number, trained on the same audio samples above. 

My main challenge will be training the Markov model, and fitting the generated patterns to work with the conductor. I will also incorporate manual controls. By default, the beat pattern will continue on its own, but the user can stop the pattern and loop a measure for a few bars if desired, then continue on with the pattern. The user will also be able to control the length of the repeated sequence (one or multiple measures), and control the volume of certain drum parts (e.g. make the bass louder or take out the hi hat). 
