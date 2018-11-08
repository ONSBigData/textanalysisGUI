# textanalysisGUI
Python web GUI for text analysis purposes. 

Purpose:
  The ONS holds staff talks from time to time, the audience, when including viewers on skype totals around 1000 participants. After the talks participants are invited to share their veiws via a survey - hosted by Survery Monkey. The questions on the survey include both questions with discrete answer options and more open ended questions that invite a response in the form of a body of text. It is questions of the latter type that this dash app analyses. Currently, all analysis of these answers is done by hand, catagorising them by topic and then determining sentiment. The dash app is intednded to replace this process to some extent.
  
What it does:
  1. The dash app takes the Survey Monkey excel file as an input via an upload. if a file that is not in ecel format is uploaded the GUI displays an error message
  2. The questions are then displayed in a table. 
  3. A button must then be pressed to propegate the question options to a drop down list.
  4. Users may then select which questions they want to have analysed. 
  5. Of the questions selected that do require the textual answers, the sentiment is analysed for each individual answer using Vader sentiment analyser. displaying the average compound score. Additionaly, a comment about the average sentiment of the anwers is displayed e.g 'overwhelmigly negative' etc.
  6. A word cloud that visualises the frequency of words used in the answers for eeach question is displayed.
  7. A box plot for each questions sentiment is displayed. Hovering over a point in the box plot displays the text that was analysed and the score it was given.  
  8. Finally, a pie chart that displays the percentages of positive, negative and neutral sentiment is displayed for the last question that was selected in the dropdown list only. 
  
How far we got:
  - We require more input from the buisness area that hosts the staff talks to find out what they really want the GUI to do. 
  - Vader sentiment analyser is used straight out of the box to analyses the sentiment we want to eventaully use Bubblebee instead as we think this might be better. 
  - Would be better to have pie charts for each question analysed instead of just the last one selected. Also displaying as a bar with different sections for positive, negative and neutral would be better.
  - The box plots currenyly interpret question numbers on a continuous scale. 
  
