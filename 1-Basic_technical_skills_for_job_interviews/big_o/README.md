# Resources 
1-https://www.youtube.com/watch?v=v4cd1O4zkGw&embeds_euri=https%3A%2F%2Fapp.manara.tech%2F&embeds_origin=https%3A%2F%2Fapp.manara.tech&source_ve_path=NzY3NTg&feature=emb_yt_watermark

2-https://www.khanacademy.org/computing/computer-science/algorithms/asymptotic-notation/a/asymptotic-notation

3-https://www.youtube.com/watch?v=SHIg5UIfBnI&embeds_euri=https%3A%2F%2Fapp.manara.tech%2F&embeds_origin=https%3A%2F%2Fapp.manara.tech&source_ve_path=NzY3NTg&feature=emb_yt_watermark

4-https://www.bigocheatsheet.com/


## problems 

#### 1- [Check If Two String Arrays are Equivalent](https://leetcode.com/problems/check-if-two-string-arrays-are-equivalent/)

#### 2- [Number of Days Between Two Dates](https://leetcode.com/problems/number-of-days-between-two-dates/)

#### 3- [Power of Two](https://leetcode.com/problems/power-of-two/)
#

#### 1) [Check If Two String Arrays are Equivalent](https://leetcode.com/problems/check-if-two-string-arrays-are-equivalent/)
  
  #### Difficulty 
   ###Easy

  
  #### Realated Topic 
  ### Array - Strings

  ### Code

```
class Solution {
public:
    bool arrayStringsAreEqual(vector<string>& word1, vector<string>& word2) {
        string s={}, t={};
        for(auto e:word1)
        {
            for(auto x:e)
            {
                s+=x;
            }
        }
        for(auto e:word2)
        {
            for(auto x:e)
            {
                t+=x;
            }
        }
        return s==t;

        
    }
};
```
#

#### 2) [Number of Days Between Two Dates](https://leetcode.com/problems/number-of-days-between-two-dates/)

#### Difficulty 
   ###Easy

  
  #### Realated Topic 
    ### Math - Strings
  
 ### Code 
 ```
 class Solution {
public:
int cnt_days(string s)
{
    int y=stoi(s.substr(0,4));
    int M=stoi(s.substr(5,2));
    int d=stoi(s.substr(8));
    int days=0;
    for(int i=1971;i<y;i++)
    {
        days+=leap_years(i)?366:365;
    }
   for(int m = 1; m < M; ++m) days += days_in_month(m, y);
    return days+d;
}
bool leap_years(int year)
{
    if( (year %4  == 0 && year % 100 != 0) || year % 400 == 0)return true;
    return false;
}
 int days_in_month(int m, int year)
        { 
            if(m==1 || m==3 || m==5 || m==7 || m==8 || m==10 || m==12 ) return 31;
            if(m==2) return leap_years(year) ? 29 : 28;
            return 30;
        }
    int daysBetweenDates(string date1, string date2) {
        return abs(cnt_days(date1)-cnt_days(date2));
    }
};
```
#

#### 3) [Power of Two](https://leetcode.com/problems/power-of-two/)

#### Difficulty 
   ###Easy

  
  #### Realated Topic 
   ### Math - Bit Manipulation - Recursion
   
 ### Code 
 ```
 Math
Bit Manipulation
Recursion
```
#





