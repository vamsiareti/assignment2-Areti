# About Me

## Name: Vamsi Krishna Areti

### About Myself:
 Hai, I am Areti Vamsi Krishna. I have done my bachelors in information technology and graduated in the year 2019 from gitam university vizag.i was born and brought up in bhimavaram. I completed my schooling in Bhimavaram .  I have been moved to Vijayawada for my +1 and +2 later I have been moved to Vizag for my bachelors coming to Vizag, it is a beautiful place where we can hang out with friends. Whenever we feel bored we can skip to the beach and enjoy nature and food there. around Vizag, there are so many places to see. coming to my graduation, I am very much interested in participating in the fests but during 1st and 2nd year, I didn't get any chance to participate but later in 3rd year I got a chance to participate in the department fest where I was a volunteer for an event and also an event organiser for another event at a time I managed both the roles and later in the 4th year I was an event organiser and also a core team member in which where I am the hospitality head this time also I have managed two roles.

 ![MyProfilePicture](MyProfilePic.jpg)

---
### Foods/Drinks I'd recommend

 These are the most famous foods available in Bhimavaram.
 People go crazy for these and they all always get craving all the time.
 It is widely known that "Bhimavaram" is a centre of various foods/varieties.


|            Food               |            Location               |            Price              |
|-------------------------------|-----------------------------------|-------------------------------|
|       Mixed Biryani           |            Bhimavaram             |            INR 300            |
|       Chicken Biryani         |            Bhimavaram             |            INR 250            |
|       Goat Biryani            |            Bhimavaram             |            INR 450            |
|       Prawn Biryani           |            Bhimavaram             |            INR 400            |

---
### Pithy Quotes
> The purpose of our lives is to be happy ~ Vamsi

> All we have is now ~ Vamsi
 
 ---
 ### Code Fencing
 > Evaluating a Determinant by Gaussian elimination: to do this you add multiples of one row to another until all entries below the main diagonal are 0. The determinant (which is unchanged by these actions) is then the product of the diagonal entries. Machines can do such things for n by n matrices with n in the hundreds or thousands, but people find the exercise a bit dull.

> Expansion of a determinant  in a row or column: let the matrix M have elements mij. The first index describes the row number, the second the column number.

> M's determinant is a sum of the elements of any single row each multiplied by a factor. What factor?

[Linear Algebra - Gaussian Elimination] (https://ocw.mit.edu/ans7870/18/18.013a/textbook/HTML/chapter04/section03.html)

```
{
const double EPS = 1E-9;
int n;
vector < vector<double> > a (n, vector<double> (n));

double det = 1;
for (int i=0; i<n; ++i) {
    int k = i;
    for (int j=i+1; j<n; ++j)
        if (abs (a[j][i]) > abs (a[k][i]))
            k = j;
    if (abs (a[k][i]) < EPS) {
        det = 0;
        break;
    }
    swap (a[i], a[k]);
    if (i != k)
        det = -det;
    det *= a[i][i];
    for (int j=i+1; j<n; ++j)
        a[i][j] /= a[i][i];
    for (int j=0; j<n; ++j)
        if (j != i && abs (a[j][i]) > EPS)
            for (int k=i+1; k<n; ++k)
                a[j][k] -= a[i][k] * a[j][i];
}

cout << det;
}
```
[Code Source](https://cp-algorithms.com/linear_algebra/determinant-gauss.html)
