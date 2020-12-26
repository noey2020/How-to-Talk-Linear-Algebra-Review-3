# How-to-Talk-Linear-Algebra-Review-3

December 25, 2020

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me! 😊

- In an earlier installment of our linear algebra primer,
we saw that any matrix can be thought of as
representing a linear function.
What we'll see today is that if the matrix is square, so if
it has the same number of rows and columns, then it also
represents a quadratic function.
Today is going to be all about square matrices
and their properties.
Let's start with a special case that we saw before.
One thing we found is that if you have a vector x,
then x transpose x is just another way of writing the dot
product of x with itself, which is the length of x squared.
In fact you can also think of this as being x transpose
times the identity
times x because the identity times x is just x.
Now, the identity matrix is just a d x d square matrix.
What if instead of having the identity there, we put some
other d x d matrix in the middle?
What if we use x transpose Mx, where M is just
any arbitrary d x d matrix, what do we get?
Let's take a look, so we have x transpose that means take x
and make it into a row.
We have this matrix M, which is d x d.
Then, we have just x, which is a column.
What are the sizes?
Here we have 1 x d.
Here, we have d x 1.
When we multiply things,
we see that the inner dimensions agree
and the result is simply going to be the outer dimensions,
which is 1 x 1.
The result is just going to be a single number as we
expected from the case of x transpose x.
The result is a single number and in fact, I'll give you a
formula for the number.
It turns out that if you just expand this out, it's quite
simple to do.
It turns out to be the sum
over all i and j
of Mij
Xi
Xj.
This is a quadratic function of x.
Each of these terms, it's a sum of a whole bunch of terms.
Each of these terms has got some Mij.
That's just a number from the matrix M, some number like
two, three, four and so on,
but the dependence on x is quadratic.
They're pairs of terms from x, Xij
or also some terms like Xi squared.
Let's see a specific example
of this just to drive the point home.
What if we have a matrix that's two by two, what kind of
quadratic function does this represent?
Well, if the matrix is two x two, these vectors x have to
be two-dimensional.
The function we're talking about is x1 x2 times this
matrix
times x1 x2
and we can just expand this out.
Let's start by doing this part.
We'll copy over the x1 x2 and let's just simplify the
matrix times the vector, what do we get?
We get
x1 plus 2x2
and 3x2.
Now, we're multiplying together these two
and this is just a single dot product.
It is x1 squared
plus
2x1
x2
plus
3x2
squared.
This is certainly a quadratic function.
All the terms in here are quadratic, x1 squared, x1 x2,
x2 squared.
Let's actually go back and see how the squares with the
formula I gave you earlier, this whole thing with the sum
over ij of Mij, let's just copy that down and see that we
actually get the same thing.
I said that it should work out to Nij
xi
xj,
the sum over all ij.
What are i and J in this case, well it's just
two-dimensional, so they're going to run over one and two.
This is equal to M11
x1 x1.
Let's just write out all the terms M12 x1 x2,
M21
x2 x1
plus
M22
x2 x2.
Now, we can go in and plug in the entries
from the matrix M.
What's M11 that's 1,
so it's x1 squared.
What's M12 that's this entry over here.
It's a 2
plus 2x1x2.
What is M21 that's a zero
and M22 was a three.
You can see that it's exactly the formula we got simply by
expanding out and in fact that's how you get this summation.
If you just do what we did before, but in greater
generality, you allow it to be d dimensional and you
allow M to just consist of variables
that haven't been defined yet.
Here is a summary of the formula.
If you start with any square matrix M, you can define a
quadratic function by
mapping x,
a d dimensional vector to
the number x transpose Mx and it works out to this
summation over here.
The summation actually lets us read out the quadratic
function very easily.
For example, we have this matrix, what if the quadratic
function associated with it, it's something that sends three
dimensional vectors to a single number, so
the three dimensional vectors x1 x2 x3
and they get sent to what number?
Well M11
is one
times
x1 squared.
Then, we have M22
times x2 squared.
Then, we have
M31
times x3 x1.
Then, we have M32
times x3 x2.
Then, we have M33
times x3
x3.
That is the quadratic function associated with this matrix.
We can also try to reverse engineering things.
Here we have a quadratic function
that takes a two dimensional vector
and just returns a number, how do we
write this function using a matrix?
What is the matrix that corresponds to this?
Well, these are two dimensional vectors, so we're going to
need a two by two matrix.
We have to fill in these four entries over here.
Now, just from the fact that the leading coefficient here
is a one, we know that this must be a one.
From the fact that this coefficient for x2 squared is a
three, we know that this must be a three,
but it's not clear what these two numbers have to be.
Let's just call them a and b.
What we know is that a plus b has to be equal to two.
There are actually several ways to achieve this function.
We could use a matrix like
1 2
0 3
or we could use 1 1
1 3
or we could use 1 0
2 3
and so on.
There are actually infinitely many possibilities.
There are many matrices that realize this particular
quadratic function.
We've been talking about square matrices, a special type of
square matrix is one that is symmetric, one that is equal
to its transpose.
What this means is that the matrix remains the same if you
reflect it in the diagonal.
Here's an example of a symmetric matrix.
If you reflect it in the diagonal, two comes back two,
three comes back to three, five comes back to five,
so it's symmetric.
The second matrix over here is not symmetric.
Look at this one and two for example.
This is a non-symmetric matrix.
It turns out that many of the matrices we'll be dealing
with will just automatically turn out to be symmetric and
this will simplify things quite a bit.
Now, an extra special case of a symmetric matrix is one
that is diagonal,
a matrix whose only nonzero entries are
along the principal diagonal, so one like this.
Diagonal matrix
is zero everywhere except along
this diagonal over here
and as a result, there's a very compact
way of writing such matrices since
there's no point using D
squared entries since most of them are zero.
We sometimes just use this shorthand over here.
Now,
one of the key quantities associated with the square
matrix is the determinant.
If we have a matrix A, the determinant is just some number
and we represent it using these bars.
We put these bars around A and you might remember from high
school or
early college that the determinant of a two by
two matrix
a b c d
is ad minus bc.
For example, if we have this two by two matrix over here,
the determinant of A
is 3 times 2
minus 1 times 1, which is 5.
It seems a little bit random.
Does the determinant actually mean anything?
It turns out that it does.
Let's look at this specific matrix.
Let's think of the rows of the matrix as being data points,
so we have these two data points and let's just go ahead
and plot these points.
We have one, two, three, four, five, six
one, two, three, four,
five, six.
The first point is three one.
The second point is one, two.
We've gone ahead and we've plotted those two points.
Now, let's take these two points and extend them to get a
full parallelogram.
We had this three one and now we take another one two and
we come out here.
Now, we have a parallelogram.
What is the area of this parallelogram?
It turns out to be five.
That's what the determinant is.
If you think of each row of the matrix as being a data
point and you plot those points
and you create the
parallelogram, the determinant is the area of the
parallelogram.
This works not just in two dimensions.
It works in d dimensions as well.
If you have a d x d square matrix, you look at the rows of
that matrix.
You plot those points in d dimensional space.
You extend them into a parallelogram.
When it's in higher dimension, instead of being called a
parallelogram, it's called a parallelepiped, so extend it
into a parallelepiped.
The volume of that object is the determinant of the matrix.
Let's actually go ahead and check that
with an example that looked familiar to us, what
if we take a three x three matrix?
Like let's take this matrix over here.
Let's go ahead and plot these points in 3D.
Let's say a, b and c are positive.
We have our three axes,
x1,
x2.
I'll just draw the third axis over here x3.
Along the x1 axis, our first point lies along the x1 axis,
it's a.
Our second point lies along the x2 axis, it's b over here
and our third point lies along the x3 axis,
so it's c over here.
Now, we extend this
into a three dimensional body.
Not very good artwork I'll confess.
What is the volume of this thing?
Well, we know this, the volume of this is just abc.
Now, let's go back to what we were
saying about determinants.
Is the determinant of this matrix abc?
Indeed it is, the determinant of a diagonal matrix is just
the product of the diagonal elements.
A very important quantity associated with the square matrix
is the inverse.
If you have a square matrix, a d x d matrix A, the inverse
is some other matrix B
such that A times B is the identity
and B times A is the identity.
What this means among other things is that B has to also be
a d x d matrix.
The notation we'll use or that we'll call this matrix B,
we'll just call it A to the minus 1, the inverse of A.
Let's do a little bit of an example.
Here's the two by two matrix A and
I'm claiming that this
particular matrix is the inverse of A.
Let's check and see if this is really the case, so
1,
2,
minus 2, zero that's A and the thing that I'm claiming is
the inverse is zero minus half,
1/2 and 1/4.
Let's see what this multiplies out to.
The first row of A times the first column of B, so we get 1.
The first row of A times the second column of B, we get
negative 1/2, plus 1/2 that's zero.
The second row of A time's the first column of B,
we get zero.
The second row of A times the second column of B, we get
one plus zero one,
which is indeed the identity matrix.
This is the inverse.
Now, there are a few things about inverses that really
should be emphasized.
First of all, they don't always exist.
There are many square matrices that don't have an inverse
and we call those matrices singular.
A matrix is singular
if it's not invertible.
It's something fairly common.
The second thing is that there's an easy way
to assess singularity.
A matrix is singular if it's determinant is zero.
Another way to put it is a matrix is invertible if and only
if its determinant is nonzero.
Now, let's look at a special case.
Suppose we have a diagonal matrix a1 to ad,
what is its inverse?
We have a diagonal matrix a1 to ad.
If you remember the notation, it means that this is the
matrix we're talking about.
All the entries off the diagonal are zero.
It's a d by d matrix.
First of all, can a matrix like this ever be singular,
non-invertible?
Yes, it can.
If you recall the determinant of a matrix like this, it's
just the product of all the diagonal entries.
It's a1
times a2 all the way to ad.
We want this product to not be zero.
We need
all the ai to be nonzero.
If that's the case, then the determinant is not zero and
the matrix is invertible.
What is the inverse?
Well, it's very simple, you just invert each of the
diagonal entries.
That's the overall inverse of the matrix.
Well that's it for the third installment of our linear
algebra primer.
This is going to hold us for a little while, so we'll give
it a week or two to sink in and then, we'll come back in a
little while and do a little bit more linear algebra.

I included some posts for reference.

https://github.com/noey2020/How-to-Talk-Linear-Algebra-Review-2

https://github.com/noey2020/How-to-Talk-Linear-Algebra-Review-1

https://github.com/noey2020/How-to-Talk-2D-Generative-Modeling

https://github.com/noey2020/How-to-Talk-Probability-Review-3

https://github.com/noey2020/How-to-Talk-Probability-Review-2

https://github.com/noey2020/How-to-Talk-Generative-Modeling-in-One-Dimension

https://github.com/noey2020/How-to-Talk-Probability-Review-1

https://github.com/noey2020/How-to-Talk-Generative-Approach-to-Classification

https://github.com/noey2020/How-to-Talk-of-Fitting-a-Distribution-to-Data-

https://github.com/noey2020/How-to-Talk-of-Host-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-of-Useful-Distance-Functions

https://github.com/noey2020/How-to-Talk-of-Improving-Nearest-Neighbor

https://github.com/noey2020/How-to-Talk-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-Matlab-Tricks-and-Tweaks

https://github.com/noey2020/How-to-Talk-Trading-and-Investing

https://github.com/noey2020/How-to-Work-in-Matlab-Development-Environment

https://github.com/noey2020/How-to-Talk-Vaccines

https://github.com/noey2020/How-to-Talk-Regression-in-Matlab

https://github.com/noey2020/How-to-Get-Started-in-Matlab

https://github.com/noey2020/How-to-Convert-Data-from-Web-Service-Using-Matlab

https://github.com/noey2020/Quote-for-the-Day

https://github.com/noey2020/How-to-Talk-Good-Investment-Strategy

https://github.com/noey2020/How-to-Talk-of-Good-Plan

https://github.com/noey2020/Thought-for-the-Day

https://github.com/noey2020/How-to-Talk-Stock-Watch-of-the-Day

https://github.com/noey2020/How-to-Talk-Data-Science

https://github.com/noey2020/How-to-Talk-Fundamental-Analysis

https://github.com/noey2020/How-to-Read-Company-Profiles

https://github.com/noey2020/How-to-Import-Data-from-Spreadsheets-and-Text-Files-Matlab-Without-Coding

https://github.com/noey2020/How-to-Talk-Model-of-Stock-Market-Prices-

https://github.com/noey2020/How-to-Talk-Digital-Wallets

https://github.com/noey2020/How-to-Talk-Investing

https://github.com/noey2020/How-to-Double-Your-Money-in-5years

https://github.com/noey2020/How-to-Talk-Matlab

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!
