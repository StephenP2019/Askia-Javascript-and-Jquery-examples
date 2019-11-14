DelayedNext

Task: The client requested the navigation buttons were hidden for a specific time (in the example the duration is 20 seconds).
Solution: Using jQuery and some basic CSS we can hide the navigation (comprised of a back and next button). I thought it would also be useful to display a timer on screen so the respondent was aware that the navigation was intentionally hidden.
Problems encountered: Pressing enter would still allow an respondent to skip past the screen, line 9 was implemented to disable this.

VideoTimer
Task: The client had requested we track how long each respondent had viewed a video.
Solution: Using the Vimeo api and jQuery we can track exactly how long a respondent has viewed the video and store this information in a hidden numeric input (stored in the live data as a question). In the example we want the respondent to watch at least 40 seconds.
Problems encountered: Initially the counter could be duplicated by skipping forward in the video as this would count as another instance of the video being played. Lines 23, 30 and 36 were introduced to ensure the timer only started if it wasn't already running. The client requested the video submit at the end if the respondent had watched enough, the function at line 39 was introduced to do this.
