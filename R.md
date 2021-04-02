inline r code must be have space before $
$\tau=$ `r tau` works. $\tau=$`r tau` does not work.

if..else.., else has to be in the same line as the closing bracket of if

rowid_to_column(df) # adds a new ID column called rowid, this is useful if we want to sample based on row id.

ggplot(data, aes(x, y, ...))+...
The initial aes is like a master configuration that can be overwritten later. For example, 
	- geom_line() fits a line through the points given in initial aes
	- geom_line(aes( y=1:10)) will use x in initial aes and y 
	- geom_line(aes( x=1:10, y=1:10)) will use new x and y 

knitting error debugging:
1. make sure pdf of the same name is closed
2. check for illegal characters, /delta which is copied from somewhere outside of R, or chinese characters.
3. check minus sign
4. check $formula$, should have no gap right before and after the $ sign

matrx fill by column because it's often created with data in the format of single vector of multivariable data 

Python pdf rendering issues
_=ax.plot(...) :use _ to hold the result, otherwise, the plotting details show in the pdf
{python, echo=FALSE} if you want to print out some results without showing codes.

paste() concatenate variables and strings

pipeline use dot as placeholder
iris %>% subset(1:nrow(.) %% 2 == 0)
3 %>% rnorm(1,.)

Python
use Anaconda instead of mini_conda for r.
when knitting to pdf: “could not find or load the Qt platform plugin windows”
I tried the following at Anaconda's prompt, and it solved this problem:
> conda remove qt
conda remove pyqt 
conda install qt 
conda install pyqt