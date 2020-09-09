# Shorcuts and code snippets 

**Rstudio Shortcuts:**   
Alt + - (the minus sign) = ` <- ` think "gets"   
Ctrl+Shift+C = Comments and de(comments) selected lines with `#`  
Ctrl+Shift+M  = the pipe `%>%` think "then"  
Ctrl + Shift + R  is an easy way to create foldable comment sections in your code



Copy a table from R to excel
write.table(x, "clipboard", sep = "\t", row.names= FALSE) 

Putting your password in a string isn't safe! Rstudio gives this handy option:
pw = rstudioapi::askForPassword("Enter Password")


Camel case (stylized as camelCase; also known as camel caps or more formally as medial capitals) is the practice of writing phrases such that each word or abbreviation in the middle of the phrase begins with a capital letter, with no intervening spaces or punctuation

Snake case is the practice of writing compound words or phrases in which the elements are separated with one underscore character and no spaces, with each element's initial letter usually lowercased within the compound and the first letter either upper- or lowercase-as in "foo_bar" and "Hello_world"

Low p-value reject the null hypothesis


bookdown::render_book("index.Rmd", bookdown::epub_book())

Atom = Open a rendered version of the Markdown in the current editor with `ctrl-shift-m`. [here](<https://atom.io/packages/markdown-preview>)

df1 <- tidyr::separate(heatmap, Response.URL, c("x1","x2"), sep = "ln=")  


The function library() will show every package and its version installed in our computer
However it is too much information
We can create a vector with the name of the packages to check later if a package is in it  
my_packages <- library()$results[,1]  
p <- as.data.frame(my_packages)  
data.table::fwrite(p, "pacakges.txt")  


Randomized Complete Block Designs (RCBD)
the purpose of blocking an experiment is to make the experimental groups more like one another. Groups are blocked by a variable that is known to introduce variability that will affect the outcome of the experiment but is not of interest to study in the experiment itself.

A rule of thumb in experimental design is often "block what you can, randomize what you cannot", which means you should aim to block the effects you can control for (e.g. sex) and randomize on those you cannot (e.g. smoking status). Variability inside a block is expected to be fairly small, but variability between blocks will be larger.


In traditional analyses if an error was made with the original data, we'd need to step through the entire process again: recreate the plots and copy-and-paste all of the new plots and our statistical analysis into your document. This is error prone and a frustrating use of time. We'll see how to use R Markdown to get away from this tedious activity so that we can spend more time doing science.

computational reproducibility. This refers to being able to pass all of one's data analysis, data-sets, and conclusions to someone else and have them get exactly the same results on their machine. This allows for time to be spent interpreting results and considering assumptions instead of the more error prone way of starting from scratch or following a list of steps that may be different from machine to machine.

Confounding Variables
In statistics, a confounder is a variable that influences both the dependent variable and independent variable, causing a spurious association. Confounding is a causal concept, and as such, cannot be described in terms of correlations or associations

In statistics, a spurious relationship or spurious correlation is a mathematical relationship in which two or more events or variables are associated but not causally related, due to either coincidence or the presence of a certain third, unseen factor (referred to as a "common response variable", "confounding factor", or "lurking variable"). 

Power Analysis
Power: The probability of rejecting the null hypothesis when the null is false 
