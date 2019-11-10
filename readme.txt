How to use it:
1. Create a new Vue project
$ vue create plotter

2. After the project is created, open the 'plotter' folder and replace the folder 'src' with the one in my zip file.

3. Now you can write commands in the textarea and click the button Plot to make svg figures.



Specification:
1. Draw a rectangle:
r <X> <Y> <Width> <Height>

2. Draw a circle:
c <CX> <CY> <Radius>

3. Draw a polygon:
p <X1,Y1> <X2,Y2> ... <Xn, Yn>



I have tried to make the commands as tolerant as possible like default commands in the textarea except that:
1. Each command should start with a legal character.
2. Only integer numbers are acceptable.

Example:
p 200,10 250,190 160,210
c 20 100 20
r 100 50 25 25
r 50 150 50 25

Or:
p   200  ,10                250,  190 160 , 210  
 
c          20  100  20
r 100   50            25  25  
R  50 150  50 25  