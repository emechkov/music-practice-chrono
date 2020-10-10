# music-practice-chrono
Tool that helps you tracking how much time did you really play music.

Demo here: https://mechkov.fr/music-practice-chrono/  
Demo displaying frequencies: https://mechkov.fr/music-practice-chrono/?show-frequencies=1

**Why did I do this?**

Well my daughter chose to learn to play the violin.  
But even though it was her choice and I might say she's pretty good at playing it, she has trouble practicing as much time as her teacher tells her to.  
If I just told her that it's time to practice for half an hour, she would make anything to actually play the violin for only five or ten minutes during this half hour.  
So... in the end it was hard to tell how much time she actually practiced her instrument.  
At some point I thought that maybe my programming skills could help her somehow to make her practice more effective.  
That's how I ended up doing this simple music practice stopwatch.  
It's not a magic wand that makes her want to practice more, but... at least we can clearly see what has been done or not...

**How to use it?**

* click on the "Start" button in the top right corner or press the **spacebar** key on your keyboard.
* when prompted, grant permission to use your device's microphone. If you don't, this tool will be pretty useless ;)
* the webapp will then start recording audio and display some usefull info: volume bar chart, practice time and effiency.

If you want to stop recording because, for example, it's lunchtime, and you want to continue practicing after without loosing "Efficiency", then:
* click on the "Pause" button in the top right corner or press the **spacebar** key on your keyboard.

To resume practicing when you come back from your break:
* click on the "Resume" button in the top right corner or press the **spacebar** key on your keyboard.

You can change the app's sensibility in the top left corner of the page. By default it's set at 150, it worker pretty well for my daughter's violin practice, but you might need to adapt this value to your instrument.  
You can change this value anytime during the practice, the "Practice time" and "Efficency" will update accordingly.  
You can see this level as a background color in the volume bar chart, to help you find the right level for your practice.

**How it works?**

If you're curious about how it actually works, you can try adding `?show-frequencies=1` at the end of the page url.  
This will show you a real-time volume/frequency bar chart.  
Then you can try to make different sounds, compare what it looks like when you make a very loud "Shhhhh" sound to what it looks like when you play your instrument.  
I didn't want to spend to much time on a complex algorithm but I still wanted to make the difference between noise and music.  
So, looking at this volume/frequency chart I decided to use the difference between the max volume and the average.  
A noise will most likely have almost the same volume for all the frequencies, so this diference will be close to zero.  
But for music, you see high peeks so this difference should be huge.  
That's pretty much it, not perfect, but works for what I needed.

Hope it will help you or your child practice more efficiently.
