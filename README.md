# Hollywood-Movies-dashboard-
Hollywood Movies 2007 to 2011
This dashboard was created  using clean data set from R 
The dash board shown the  rating   of  of  different movies using Rotten tomato
The Most profitable  Studio was  also analysed 
This dataset contain information Movies 
[my dashborad](https://app.powerbi.com/links/b0ZO7IUrJc?ctid=6efd0f20-57c8-4447-b53f-00d4992ca50b&pbi_source=linkShare)

> #Load data
> 
> df<- read.csv(“https://public.tableau.com/app/sample-data/HollywoodsMostProfitableStories.csv")
Error: unexpected input in "df<- read.csv(“"
> #Load data
> df<- read.csv(“https://public.tableau.com/app/sample-data/HollywoodsMostProfitableStories.csv")
Error: unexpected input in "df<- read.csv(“"
> df<- read.csv("https://public.tableau.com/app/sample-data/HollywoodsmostprofitableStories.csv")
Error in file(file, "rt") : 
  cannot open the connection to 'https://public.tableau.com/app/sample-data/HollywoodsmostprofitableStories.csv'
In addition: Warning message:
In file(file, "rt") :
  cannot open URL 'https://public.tableau.com/app/sample-data/HollywoodsmostprofitableStories.csv': HTTP status was '404 Not Found'
> load("~/.RData")
> df<- read.csv("https://public.tableau.com/app/sample-data/HollywoodsMostProfitableStories.csv")
> df
                                  Film     Genre           Lead.Studio Audience..score.. Profitability
1                           27 Dresses    Comedy                   Fox                71     5.3436218
2                 (500) Days of Summer    Comedy                   Fox                81     8.0960000
3                   A Dangerous Method     Drama           Independent                89     0.4486447
4                        A Serious Man     Drama             Universal                64     4.3828571
5                  Across the Universe   Romance           Independent                84     0.6526032
6                            Beginners    Comedy           Independent                80     4.4718750
7                            Dear John     Drama                  Sony                66     4.5988000
8                            Enchanted    Comedy                Disney                80     4.0057371
9                            Fireproof     Drama           Independent                51    66.9340000
10                    Four Christmases    Comedy          Warner Bros.                52     2.0229250
11          Ghosts of Girlfriends Past    Comedy          Warner Bros.                47     2.0444000
12                   Gnomeo and Juliet Animation                Disney                52     5.3879722
13                  Going the Distance    Comedy          Warner Bros.                56     1.3140625
14                     Good Luck Chuck    Comedy             Lionsgate                61     2.3676851
15         He's Just Not That Into You    Comedy          Warner Bros.                60     7.1536000
16  High School Musical 3: Senior Year    Comedy                Disney                76    22.9131365
17           I Love You Phillip Morris    Comedy           Independent                57     1.3400000
18                    It's Complicated    Comedy             Universal                63     2.6423529
19                           Jane Eyre   Romance             Universal                77            NA
20                         Just Wright    Comedy                   Fox                58     1.7974167
21                             Killers    Action             Lionsgate                45     1.2453333
22                          Knocked Up    Comedy             Universal                83     6.6364018
23                           Leap Year    Comedy             Universal                49     1.7152632
24                   Letters to Juliet    Comedy                Summit                62     2.6393333
25                      License to Wed    Comedy          Warner Bros.                55     1.9802064
26                  Life as We Know It    Comedy           Independent                62     2.5305263
27                  Love & Other Drugs    Comedy                   Fox                55     1.8176667
28                        Love Happens     Drama             Universal                40     2.0044444
29                       Made of Honor    Comedy                  Sony                61     2.6490683
30                          Mamma Mia!    Comedy             Universal                76     9.2344539
31                       Marley and Me    Comedy                   Fox                77     3.7467818
32                   Midnight in Paris   Romance                  Sony                84     8.7447059
33      Miss Pettigrew Lives for a Day    Comedy           Independent                70     0.2528949
34                         Monte Carlo   Romance      20th Century Fox                50     1.9832000
35                    Music and Lyrics   Romance          Warner Bros.                70     3.6474106
36                My Week with Marilyn     Drama The Weinstein Company                84     0.8258000
37                      New Year's Eve   Romance          Warner Bros.                48     2.5364286
38  Nick and Norah's Infinite Playlist    Comedy                  Sony                67     3.3527293
39                     No Reservations    Comedy                                      64     3.3071804
40                   Not Easily Broken     Drama           Independent                66     2.1400000
41                             One Day   Romance           Independent                54     3.6827333
42                  Our Family Wedding    Comedy           Independent                49            NA
43                  Over Her Dead Body    Comedy              New Line                47     2.0710000
44                     P.S. I Love You   Romance           Independent                82     5.1031168
45                            Penelope    Comedy                Summit                74     1.3827997
46              Rachel Getting Married     Drama           Independent                61     1.3841667
47                         Remember Me     Drama                Summit                70     3.4912500
48                    Sex and the City    Comedy          Warner Bros.                81     7.2217958
49                  Sex and the City 2    Comedy          Warner Bros.                49     2.8835000
50              She's Out of My League    Comedy             Paramount                60     2.4405000
51                  Something Borrowed   Romance           Independent                NA     1.7195143
52                             Tangled Animation                Disney                88     1.3656923
53                    The Back-up Plan    Comedy                   CBS                47     2.2025714
54 The Curious Case of Benjamin Button   Fantasy          Warner Bros.                81     1.7839437
55                         The Duchess     Drama             Paramount                68     3.2078502
56                  The Heartbreak Kid    Comedy             Paramount                41     2.1294442
57              The Invention of Lying    Comedy          Warner Bros.                47     1.7513514
58                        The Proposal    Comedy                Disney                74     7.8675000
59            The Time Traveler's Wife     Drama             Paramount                65     2.5982051
60         The Twilight Saga: New Moon     Drama                Summit                78    14.1964000
61                      The Ugly Truth    Comedy           Independent                68     5.4026316
62                            Twilight   Romance                Summit                82    10.1800270
63             Twilight: Breaking Dawn   Romance           Independent                68     6.3833636
64 Tyler Perry's Why Did I get Married   Romance           Independent                47     3.7241924
65                     Valentine's Day    Comedy          Warner Bros.                54     4.1840385
66                 Waiting For Forever   Romance           Independent                53     0.0050000
67                            Waitress   Romance           Independent                67    11.0897415
68                              WALL-E Animation                Disney                89     2.8960191
69                 Water For Elephants     Drama      20th Century Fox                72     3.0814211
70               What Happens in Vegas    Comedy                   Fox                72     6.2676470
71                        When in Rome    Comedy                Disney                44            NA
72  You Will Meet a Tall Dark Stranger    Comedy           Independent                35     1.2118182
73                     Youth in Revolt    Comedy The Weinstein Company                52     1.0900000
74          Zack and Miri Make a Porno   Romance The Weinstein Company                70     1.7475417
   Rotten.Tomatoes.. Worldwide.Gross Year
1                 40      160.308654 2008
2                 87       60.720000 2009
3                 79        8.972895 2011
4                 89       30.680000 2009
5                 54       29.367143 2007
6                 84       14.310000 2011
7                 29      114.970000 2010
8                 93      340.487652 2007
9                 40       33.467000 2008
10                26      161.834000 2008
11                27      102.220000 2009
12                56      193.967000 2011
13                53       42.050000 2010
14                 3       59.192128 2007
15                42      178.840000 2009
16                65      252.044501 2008
17                71       20.100000 2010
18                56      224.600000 2009
19                85       30.147000 2011
20                45       21.569000 2010
21                11       93.400000 2010
22                91      219.001261 2007
23                21       32.590000 2010
24                40       79.180000 2010
25                 8       69.307224 2007
26                28       96.160000 2010
27                48       54.530000 2010
28                18       36.080000 2009
29                13      105.962734 2008
30                53      609.473955 2008
31                63      206.073000 2008
32                93      148.660000 2011
33                78       15.173694 2008
34                38       39.664000 2011
35                63      145.896422 2007
36                83        8.258000 2011
37                 8      142.040000 2011
38                73       33.527293 2008
39                39       92.601050 2007
40                34       10.700000 2009
41                37       55.241000 2011
42                14       21.370000 2010
43                15       20.710000 2008
44                21      153.093505 2007
45                52       20.741996 2008
46                85       16.610000 2008
47                28       55.860000 2010
48                49      415.253258 2008
49                15      288.350000 2010
50                57       48.810000 2010
51                NA       60.183000 2011
52                89      355.080000 2010
53                20       77.090000 2010
54                73      285.431000 2008
55                60       43.305978 2008
56                30      127.766650 2007
57                56       32.400000 2009
58                43      314.700000 2009
59                38      101.330000 2009
60                27      709.820000 2009
61                14      205.300000 2009
62                49      376.661000 2008
63                26      702.170000 2011
64                46       55.862886 2007
65                17      217.570000 2010
66                 6        0.025000 2011
67                89       22.179483 2007
68                96      521.283432 2008
69                60      117.094000 2011
70                28      219.367646 2008
71                15       43.040000 2010
72                43       26.660000 2010
73                68       19.620000 2010
74                64       41.941000 2008
> view(df)
Error in view(df) : could not find function "view"
> View(df)
> install.packages("tidyverse")
WARNING: Rtools is required to build R packages but is not currently installed. Please download and install the appropriate version of Rtools before proceeding:

https://cran.rstudio.com/bin/windows/Rtools/
Installing package into ‘C:/Users/esekh/AppData/Local/R/win-library/4.2’
(as ‘lib’ is unspecified)
trying URL 'https://cran.rstudio.com/bin/windows/contrib/4.2/tidyverse_2.0.0.zip'
Content type 'application/zip' length 430757 bytes (420 KB)
downloaded 420 KB

package ‘tidyverse’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
	C:\Users\esekh\AppData\Local\Temp\RtmpuuHIGv\downloaded_packages
> 
> #Load library:
> install.packages("tidyverse")
WARNING: Rtools is required to build R packages but is not currently installed. Please download and install the appropriate version of Rtools before proceeding:

https://cran.rstudio.com/bin/windows/Rtools/
Installing package into ‘C:/Users/esekh/AppData/Local/R/win-library/4.2’
(as ‘lib’ is unspecified)
trying URL 'https://cran.rstudio.com/bin/windows/contrib/4.2/tidyverse_2.0.0.zip'
Content type 'application/zip' length 430757 bytes (420 KB)
downloaded 420 KB

package ‘tidyverse’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
	C:\Users\esekh\AppData\Local\Temp\RtmpuuHIGv\downloaded_packages
> install.packages("tidyverse")
WARNING: Rtools is required to build R packages but is not currently installed. Please download and install the appropriate version of Rtools before proceeding:

https://cran.rstudio.com/bin/windows/Rtools/
Installing package into ‘C:/Users/esekh/AppData/Local/R/win-library/4.2’
(as ‘lib’ is unspecified)
trying URL 'https://cran.rstudio.com/bin/windows/contrib/4.2/tidyverse_2.0.0.zip'
Content type 'application/zip' length 430757 bytes (420 KB)
downloaded 420 KB

package ‘tidyverse’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
	C:\Users\esekh\AppData\Local\Temp\RtmpuuHIGv\downloaded_packages
> install.packages("tidyverse")
WARNING: Rtools is required to build R packages but is not currently installed. Please download and install the appropriate version of Rtools before proceeding:

https://cran.rstudio.com/bin/windows/Rtools/
Installing package into ‘C:/Users/esekh/AppData/Local/R/win-library/4.2’
(as ‘lib’ is unspecified)
trying URL 'https://cran.rstudio.com/bin/windows/contrib/4.2/tidyverse_2.0.0.zip'
Content type 'application/zip' length 430757 bytes (420 KB)
downloaded 420 KB

package ‘tidyverse’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
	C:\Users\esekh\AppData\Local\Temp\RtmpuuHIGv\downloaded_packages
> str(df)
'data.frame':	74 obs. of  8 variables:
 $ Film             : chr  "27 Dresses" "(500) Days of Summer" "A Dangerous Method" "A Serious Man" ...
 $ Genre            : chr  "Comedy" "Comedy" "Drama" "Drama" ...
 $ Lead.Studio      : chr  "Fox" "Fox" "Independent" "Universal" ...
 $ Audience..score..: int  71 81 89 64 84 80 66 80 51 52 ...
 $ Profitability    : num  5.344 8.096 0.449 4.383 0.653 ...
 $ Rotten.Tomatoes..: int  40 87 79 89 54 84 29 93 40 26 ...
 $ Worldwide.Gross  : num  160.31 60.72 8.97 30.68 29.37 ...
 $ Year             : int  2008 2009 2011 2009 2007 2011 2010 2007 2008 2008 ...
> 
> colSums(is.na(df))
             Film             Genre       Lead.Studio Audience..score..     Profitability Rotten.Tomatoes.. 
                0                 0                 0                 1                 3                 1 
  Worldwide.Gross              Year 
                0                 0 
> df <- na.omit(df)
> colSums(is.na(df))
             Film             Genre       Lead.Studio Audience..score..     Profitability Rotten.Tomatoes.. 
                0                 0                 0                 0                 0                 0 
  Worldwide.Gross              Year 
                0                 0 
> 
> dim(df[duplicated(df$Film),])[1]
[1] 0
> 
> df$Profitability <- round(df$Profitability ,digit=2)
> 
> df$Worldwide.Gross <- round(df$Worldwide.Gross ,digit=2)
> dim(df)
[1] 70  8
> 
> library(ggplot2)
> 
> ggplot(df,aes(x=Profitability y=Worldwide.Gross)) + geom_boxplot(outlier.colour = "red", outlier.shape = 1)+ scale_x_continuous(labels = scales::comma)+coord_cartesian(ylim = c(0, 1000))
Error: unexpected symbol in "ggplot(df,aes(x=Profitability y"
> ggplot(df,aes(x=Profitability, y=Worldwide.Gross))+geom_boxplot(outlier.colour= "red",outlier.shape= 1)+scale_x_continuous(labels = scales::comma)+coord_cartesian(ylim= c(0,1000))
Warning message:
Continuous x aesthetic
ℹ did you forget `aes(group = ...)`? 
> 
> Q1 <- quantile(df$Profitability, .25)
> Q3 <- quantile(df$Profitability, .75)
> 
> IQR <- IQR(df$Profitability)
> 
> no_outliers <- subset(df, df$Profitability> (Q1 - 1.5*IQR) & df$Profitability< (Q3 + 1.5*IQR))
> 
> 
> dim(no_outliers)
[1] 65  8
> 
> Q1 <- quantile(no_outliers$Worldwide.Gross, .25)
> Q3 <- quantile(no_outliers$Worldwide.Gross, .75)
> IQR <- IQR(no_outliers$Worldwide.Gross)
> 
> df1 <- subset(no_outliers, no_outliers$Worldwide.Gross> (Q1 - 1.5*IQR) & no_outliers$Worldwide.Gross< (Q3 + 1.5*IQR))
> dim(df1)
[1] 61  8
> dim(df1)
[1] 61  8
> ggplot(df1, aes(x=Lead.Studio, y=Rotten.Tomatoes..)) + geom_point()+ scale_y_continuous(labels = scales::comma)+coord_cartesian(ylim = c(0, 110))+theme(axis.text.x = element_text(angle = 90))
> 
