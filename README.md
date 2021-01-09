# Introduction

This repo contains the notebooks with the comprehansive EDA and data-driven insights from the data collected in Kaggle's 2020 survey of 'State of Data Science and Machine Learning 2020' (https://www.kaggle.com/c/kaggle-survey-2020).

There are two principal notebooks here as follows

- *Kaggle 2020 Survey - Associated Insights.ipynb* - the notebook with the world-wide trends analytics
- *Ukrainians on Kaggle 2020.ipynb* - the same analytics yet performed for Ukrainian community of Kaggle 2020 survey participants

The sections below are mainly centric around global insights and projections captured in *Kaggle 2020 Survey - Associated Insights.ipynb*

As expected, the insights, although referred to as 'State of Data Science and Machine Learning 2020', will be somewhat driving the trends in Data Science and ML industry in the next two years.

# Executive Summary

This notebook is intended to provide the comprehansive EDA and data-driven insights from the data collected in Kaggle's 2020 survey of **'State of Data Science and Machine Learning 2020'**.

It contains several chapters dedicated to various topics covered by the survey.

**Chapter 1** provides the comprehensive outlook on the demographical and generic experience profile of the survey repondents in terms of their

- Age
- Gender
- Level of Education
- Occupation
- Years of Programming Experience
- Years of ML Experience

**Chapter 2** conveys some insights on the technical skills of the kagglers. It is not extensive due to the number of high-quality notebooks already dedicated to this topic (see some links in the **References** section below). Instead of investing more time into analysis of this type, I spent it on analytics in the areas where less attention has been paid by other contest participants (see details in Chapters 3-6  below). 

However, there are still interesting discoveries found due to research on the multi-variative categorical feature associations (*spoiler*: there is a forecast about when and how *Julia revolution* in Data Science could happen). 

**Chapter 3** is concentrated on the organizational environment and job responsibilities of the survey participants. These are

- Size of the employer organization
- Size of the team working in Data Science-related areas
- Adoption of ML in the organization
- Individual job responsibilities of the survey participants
- Spending on ML and Cloud Computing in the last 5 years

From that stand-point, it describes the essential business landscape where kagglers operate on the daily basis.

**Chapter 4** is focused on the preferences of Cloud Computing Provider usage by Kagglers. It draws insights on the popularity of cloud computing platforms and products among the survey participants who are professionals (as opposed to non-professionals - see the note below). In particular, it covers

- Cloud Platforms usage
- Cloud Computing products usage
- Cloud ML products usage
- BigData platforms
- BI tools (mostly, the cloud-based ones)

The line of the narrative in this chapter is often attached to the good news and opportunities for the top three cloud service providers in the market as follows

- Amazon Web Services (AWS)
- Google Cloud Platform (GCP)
- Microsoft Azure Cloud (MS Azure)

**Chapter 5** is dedicated to the analysis of usage of Data Science automation tools by the survey respondents. In particular, it conveys findings regarding

- the usage of automated machine learning tools
- the usage of tools to help manage machine learning experiments

**Chapter 6** delves into details about the favorite knowledge sharing and information/knowledge acquisition channels used by the survey participants. In this chapter, we are going to analize the preferences of the survey participants as for

- platforms and tools to publicly share or deploy their data analysis or machine learning applications
- platforms to take online data science courses
- primary tools they use to analyze data
- favorite media sources that report on data science topics

**Chapter 7** provides the geographical perspective on the Kaggle 2020 survey participants. It draws a collection of maps to display by-country distribution of the participants by their demographic data, experience and usage of Cloud Service platforms.

**Appendix** at the end of the notebook contains supplementary notes on

- Methodology and technical implementation details about this notebook
- Comments on why Rapid EDA tools are not applicable to the EDA in the scope of this project
- References to the high-quality notebooks of other contest participants that inspired the work done here as well as to the blog posts explaining advanced topics of visualizing relations between categorical features

# Chapter 1: Demography and Generic Experience

This chapter will be focused on the insights about basic demographic and generic experience characteristis of the survey participants as follows

- Age
- Gender
- Level of Education
- Occupation
- Years of Programming Experience
- Years of ML Experience

## Age-Gender Relationship

We can see a number of interesting demographic insights

- the young generations (peope of the age of 18-29) predominate the population of the survey respondens, and the entire Kaggle population as of the moment, most likely
- people of the age of 25-29 is the top group within the Kaggler survey community
- males dominate over females and other genders in every age category
- the fraction of women in younger generation of Kagglers is slightly higher then in the older ones

## Age-to-Level-of-Education Relationship

We can see that there are four biggest Kaggle population clusters in the space of Education level and Age as follows

1. Bachelors of the age of 18-21 (the biggest cluster so far)
2. People of the age of 25-29 with the Master degree
3. Bachelors of the age of 22-24
4. Masters of the age of 22-24 

On top of the population cluster insight above, we can draw the additional intelligence as follows

- People with Bachelor degree predominate in more junior age groups
- In senior age groups, the percentage of Master and Doctoral degrees grows
- People with Master degrees predominate in every age group, starting from 25-29 and older.
- Starting the age group of 35-39 and older, the amount of respondents with Doctoral degrees is only a little less then the respondents with  Master degree for the same age group

Based on the facts/knowledge discoveries above, combined with my onw (quite subjective) 'kaggling' experience, I could formulate a few suggestions regarding better Kaggle community engagement/participation practices. 

1. Senior kagglers with Master and Doctoral degrees who crossed the *akme age* line (that is, those who are of the age of 45-49 and older) constitute the 'golden pool' of experts here in Kaggle platform. It could make sense to better engage with them to motivate them to do more knowledge sharing with and possibly other training activities for more junior population of Kagglers.
2. Ethical standards conduct across various activities on the platform (otherwise known as 'ethical kaggling') could be one of the pillars to keep Senior-level expertswilling to contribute to the body of knowledge here at Kaggle more. Conversly, the lack of 'ethical kaggling' may discourage them from being active on the platform.
3. Since the majority of Kagglers are quite junior, one of their motivations is to prove their competencies/expertise as well as stand out of the crowd. Some of them are yet to get their heads around the concept of 'ethical kaggling' (see the discussion threads like https://www.kaggle.com/discussion/206639 and similar).
4. Propaganda and some sort of control of conducting the 'ethical kaggling' practices can be benefitial for the Kaggle community to sustain in the long run. It will also help to better motivate the top senior-level experts to share their knowledge and wisdom with junior generations.

## Age-Occupation Relationship

As we can see, there are top clusters of the Kaggler survey respondents in the space of Age and Occupation as follows

- Students of the age of 18-21
- Students of the age of 22-24
- Students of the age of 25-29
- Data Scientists of the age of 25-29
- Data Scientists of the age of 30-34

The next tier of the responder clusters shows quite a significant amount of young unemployed people (of the age of 22-24 and 25-29, respectively). It may imply that young unemployed data science professional regard Kaggle as a platform to increase their chances to get a prominent job in the respective Data Science-related area.

Additional insigts within the Age-Occupation breakdown can be drawn as follows

- students predominate the age groups of 18-21 and 22-24, and they stop being dominant in the age group of 25-29 and older
- in the age groups of 25-29 and older, Data Scientist is the most popular occupation within the survey responders
- the occupations of Software Engineer, Data Analyst, and Research Scientist are in the next tier in terms of popularity
- quite a significant amount of responders indicated 'Other' as their occupation - it can be assumed these are professionals outside of IT/Software Development/Scient/Statistic-related fields interested in Data Science topics
- the ratio of product and project management professionals, although quite small in every age group, displays the tendency to grow up from the age group of 25-29 to 50-54
- the ratio of unemployed is still significant for middle-age and senior-age groups

## Age-to-Years-of-Programming-Experience Relationship

As we can see, the intelligence supports our naive intution about the positive correlation between the age and programming experience. More specifically we find that

the majority of young kagglers are relatively inexperienced (having up to 3-5 years of programming experience at maximum)
more senior people tend to demonstrate more years of programming experience
in every age group (even in the senior ones), there is always a tiny fraction of people who indicated no programming experience at all

## Gender-to-Level of Education Relationship

As we can see, there are top clusters of the survey respondents within the dimensions of Gender and Level of Educations as follows

- Males with Bachelor's degree
- Males with Master's degree
- Males with Doctoral degree
- Females with Bachelor's degree
- Females with Master's degree

Bachelor and Master degrees are the most common levels of education for every gender.

## Gender-to-Occupation Relationship

We find that 

- Student occupation is the most popular one among every gender
- Top three occupations (after Student) for males are Data Scientist, Software Engineer, and Other
- Top three occupations (after Student) for females are Data Scientist, Data Analyst, and Unemployed

As we can see, the ratio of unemployment among female respondents to the survey is higher.

## Gender-to-Programming Experience Relationship

We find that

- the majority of both males and females are relatively inexperienced as they fit into 3 programming experience categories (3-5 years, 1-2 years, and <1 year)
- the ratio of males having 5-10 years of experience is higher then the one of females
- the ratio of females having zero programming experience is higher then the one of males

## Gender-to-ML Experience Relationship

We see that

- the majority of the survey respondents are relatively inexperienced in ML for every gender (they fit to Under 1 year, 1-2 years, 2-3 years and 'I do not use ML ... ' categories)
- the ratio of female indicated 'I do not use ML ... ' is higher then the one of males

## Level of Education-to-Occupation Relationship

We can see the top three clusters of the survey respondents in terms of the Level of Education and Occupation

- Students with Bachelor degree
- Students with Master degree
- Data Scientists with Master degree

On top of that, we find that

- number of people with Bachelor degree exceeds the number of people with Master degree in Students and Unemployed groups
- number of people with Bachelor and Master degrees is on a par for Software Engineers
- for the rest of occupations, we see the number of people with Master degree exceeding the one with Bachelor degree

## Level of Education-to-Programming Experience Relationship

As we can see there are four top clusters among the survey responders within Education and Programming experience dimensions as follows

- People with Bachelor's degree having 1-2 years of programming experience
- People with Master's degree having 3-5 years of programming experience
- People with Bachelor's degree having 3-5 years of programming experience
- People with Master's degree having 1-2 years of programming experience

For more experienced categories (5+ years of programming experience), we find that the ratio of people with Master's degree exceeds one for Bachelor's degree.

Percentage of people with Doctoral degree is higher in the most experienced categories (programming experience of 10-20 years as well as 20+ years).

## Level of Education-to-ML Experience Relationship

As we can see, the majority of the survey participants fall into the clusters indicating relatively inexperienced professionals. These are

- People with Bachelor's degree having less then 1 year of ML experience
- People with Master's degree having less then 1 year of ML experience
- People with Bachelor's degree having 1-2 years of ML experience
- People with Master's degree having 1-2 years of ML experience

## Occupation-to-Programming Experience Relationship

As we can see, the population of the survey responders is absolutely predominated by students with a little programming experience (between 0 and 5 years).

Among non-student participants, we can see top three clusters (by the number of respondents in the cluster) as follows

- Data Scientists with 3-5 years of programming experience
- Data Scientists with 5-10 years of programming experience
- Unemployed with less then 1 year of programming experience

## Programming-to-ML Experience Relationship

As we can see, the majority of the survey participants fall into relatively inexperienced clusters as follows

- professionals with less then 1 year of programming and less then 1 year of ML experience
- professionals with 1-2 years of programming and less then 1 year of ML experience
- professionals with 3-5 years of programming and less then 1 year of ML experience
- professionals with 1-2 years of programming and 1-2 years of ML experience
- professionals with 3-5 years of programming and 1-2 years of ML experience

## Kaggler Geography

### Male Kagglers

As we can see, the top 5 countries with the largest male kagglers population (500+ respondents) within the survey respondents are as follows

- India
- USA
- Brazil
- Japan
- Russia

In the second tier of the countries with the most active male survey participats (300-500 participants) are the countries below 

- UK
- Germany
- Nigeria
- China

We also see a few countries to be slightly behind the tier 1 and tier 2 leaders in terms of participating kagglers (France, Spain, Turkey).

*Note:* it is interesting to indicate the under-represented voice of China in this survey (relative to the country population).

### Female Kagglers

As we can see, only two countries have more then 400 female kagglers who participated in the survey 2020. These are

- India
- USA

### Kagglers with Doctoral Degree

As we can see, the number of Kaggle survey responders with Doctoral degree is the highest in the US - *407* (although the US-based Kaggle survey participants population is not the largest one - please see above). The second place holds India (whose Kaggle survey participants population is the largest across the globe), with *275* kagglers with Doctoral degrees participated in the survey.

The rest of the countries have less then 200 Kagglers with Doctoral degree who responded to the survey. Still , there some countries who have between 60 and 200 Doctors responded to the survey. These are

- UK
- Germany
- Brazil
- France
- Spain
- Japan

As we can see, Nigeria, one of the countries with the highest Kaggler community, is not in the top list of countries with Doctoral degree kagglers.

### Kagglers with Master's Degree

We can see the following countries to have  more then 200 survey participants with Master's degree as follows

- India 
- USA
- Japan
- Russia
- Brazil
- China
- UK
- Germany
- France
- Spain

As we can see, Nigeria, one of the countries with the highest Kaggler community, is not in the top list of countries with Master's degree kagglers.

### Kaggle Programming Veterans

*Note:* In this post, programming veterans are considered to be the professionals with 20+ years of programming experience.

As we can see, the biggest number of programming veterans among the survey respondents reside in the US. The rest of the countries are well below the bar set by the US.


However, there are several countries that have between 60 and 100 programming veterans participated in the survey. These are

- Japan
- UK
- Brazil
- India

As we see, India, although represented by the largest population of Kagglers among the survey respondents, does not possess the huge pool of the experts with 20+ years of programming experience vs. the rest of the leading countries.

### Kaggle ML Veterans

*Note*: In this post, ML veterans are considered to be the professionals with 10-20 and 20+ years of ML experience

As we can see, the US absolutely predominates the rest of the world in terms of the number of the survey participants having 10+ years of ML experience

# Chapter 2: 'Julia Revolution' In Data Science

Per the word of some of the industry analysts, Julia is predicted to be the next big thing in the area of Machine Learning and Data Science, to gradually replace Python in the top leading positions in the next 3-5 years. However, the results of the survey shows Julia is yet to find its way to the mainstream ML and Data Science software development.

We can see that 

- Julia is experimented with by relatively experienced professionals (Data Scientists, Research Scientists, and Software Engineers with 10+ years of experience) as well as by Students
- the rest of the kaggler respondents do not display the sound interest in using Julia yet

So 'Julia revolution' is not likely to happen soon. It will only be possible to start when today's students who became funs of Julia obtain more industrial  experience as well as occupy senior-level positions to influence strategic technical and business decisions in their organizations.

# Chapter 3: Organization and Job Responsibility Profiles

In this chapter, we are going to analize the key characteristics of the employers of the survey participants. These are

- Size of the organization
- Size of the team working in Data Science-related areas
- Adoption of ML in organization
- Individual Job responsibilities of the survey participants
- Spending on ML and Cloud Computing in the last 5 years

*Note:* Per the findings of other researches, the responses to Q24, the quetion on the level of compensation (https://www.kaggle.com/dwin183287/kagglers-seen-by-continents), seem to be skewed or somewhat faked by the respondents. Therefore the analysis in this notebook won't cover it.

## Organization Size, Data Science and ML Adoption

As we can see, the largest cluster of the survey responders work for the small organizations (0-49 employees). Within that bucket, the most of the organization has either 1-2, 0 or 3-4 employees responsible for data science workloads.

The majority of such organizations is still exploring ML methods. However, some fraction of such organizations 

- is reported to recently start using ML methods, or
- do not use ML currently

Small organizations with no workers dedicated to data science workloads mostly do not use ML in their daily operations (which is a kind of expected intuition).

Interesting (small-sized) subclusters of small organizations with 5+ employees dedicated to data science workloads display mature usage of ML solutions in production.

Second and third largest clusters of survey responders constitute those who work for

- organizations with 10000+ employees
- organizations with 1000-9999 employees

In such clusters, we can see quite a lot of respondents to indicate their organizations to have well established ML methods.

Overall, irrespective to the organization size, it seems that the size of a Data Science-centric team of 5+ workers indicates certain level of ML methods maturity within an organization. In organizations in every size group, the companies with 5+ workers dedicated to Data Science activities indicated to either start using ML in production recently or have the mature ML methods established.

## Individual Job Responsibilities of the Survey Participants

As we can see, Data Scientists and Data Analysts are typically the go-to persons to analyze and understand data, regardless the employer organization size.

Aditional insights are detected as follows

- typically, the organizations of larger size hire more experienced Data Scientists and Data Analysts, involving them in the worksflows to anlize and understand the data 
- Other occupations are typically less involved in handling such a type of job responsibilities

### Analizing and Understanding Data

As we can see, Data Scientists and Data Analysts are typically the go-to persons to analyze and understand data, regardless the employer organization size.

Aditional insights are detected as follows

- typically, the organizations of larger size hire more experienced Data Scientists and Data Analysts, involving them in the worksflows to anlize and understand the data 
- Other occupations are typically less involved in handling such a type of job responsibilities

### Building and/or Running the Data Infrastructure

We can find that

- In the majority of the organizations, Data Scientists and Software Engineers are often tasked with Building and/or Running the Data Infrastructure
- In large organizations (1000+), a special role of Data Engineer is often introduced to handle such type of work in a dedicated manner (with Data Scientists and Software Engineers off-loaded to do some other core activities on their side)
- Data Analysts are sometimes  involved in building and running the data infrastructure, especially in smaller-sized organizations (however, the percentage of Data Analysts doing so in organizations of 1000-9999 employee size sounds surprinsingly high as displayed)

### Building Prototypes

We find that, regardless the size of the employer organizations, the following roles are mostly involved in building prototypes

- Data Scientists
- Software Engineers
- ML Engineers
- Research Scientists

### Building and/or Running an ML Service

As we can see, the top three roles involved in building and/or running ML Services (regardless the size of an employer organization) are

- Data Scientist
- ML Engineer
- Software Engineer

### Experimentation

As we can see, the top roles involved in experimentation (regardless the size of an employer organization) are

- Data Scientist
- Research Scientist

Sometimes ML and Software Engineers are involved in this type of activities.

### Doing Research

As we can see, the top roles involved in doing research (regardless the size of an employer organization) are

- Data Scientist
- Research Scientist

## ML Spendings

From looking at the charts, we can see the most popular  option as for ML spending is USD 0, regardless the orgranization size. It may be indicative of the inaccuracies in the responder inputs when they responded to the respective question of the survey (or otherwise they could fake the answers for a reason).

Still, if considering the meaningful responses, it looks like

- large organizations tend to spend more in ML (100+ k USD in the last 5 years)
- smaller-sized organizations spent 100-999 or 1000-9999 USD in ML in the last 5 years

# Chapter 4: Battle of Giants

In this chapter, we are going to draw insights on the popularity of cloud computing platforms and products among the survey participants who are professionals (as opposed to non-professionals - see the note below). In particular, it will cover

- Cloud Platforms usage
- Cloud Computing products usage
- Cloud ML products usage
- BigData platforms
- BI tools (mostly, the cloud-based ones)

The line of the narrative in this chapter will be often attached to the good news and opportunities for the top three cloud service providers in the market as follows

- Amazon Web Services (AWS)
- Google Cloud Platform (GCP)
- Microsoft Azure Cloud (MS Azure)

*Notes:* 

- We are specifically going to analize the responses to Q26-Q31.
- The insights in this section refer to the Kaggle community only. It may not be  representative group for the entire community of Data Scientist professionals across the globe. However, some of the conclusions below can be interesting from the marketing stand-point.
- Survey organizers defined non-professionals as students, unemployed, and respondents that have never spent any money in the cloud.

## Usage of Cloud Service Providers: By Occupation/Programming Experience View

We find that the top three list of cloud service providers among the Kaggle survey responders are

- AWS
- GCP
- MS Azure

The rest of the cloud service providers seems to loose the competitive edge toward the top three provider list above at the moment.

Also, it is notable that 'None' category slightly exceeds the size of MS Asure bar, and it means the market may not be saturated with the cloud service provider offerings.

We also see professionals with 3-5 years and 5-10 years of programming experince to be the largest group of users of the top 3 cloud service providers. More senior professionals (with 10+ years of experience) are less represented within the cloud service users on each of top 3 platforms (depending on the marketing priorities, special actions to educatesuch seniors could help to get the better spread of the cloud services).

As we can see, the majority of top three cloud service provider users fit into the roles below

- Data Scientists
- Software Engineers

The third posion is held by

- ML Engineeris (AWS, GCP)
- Data Analysts (MS Azure)

As noted earlier, 'Other' occupation group is too big itself, and it might be worth breaking it into more granular categories in the future surveys. As we see, 'Other' group takes a significant fraction of each cloud service platform users (although it is never seen in the top three list ffor any off the platforms).

### AWS Usage Patterns

We find that

- Data Scientists with 3-5 and 5-10 years of programming experience are the top user groups for AWS within the survey respondents
- In Software Engineer, ML Engineer, and Data Analyst groups, professionals with  3-5 and 5-10 years of experience predominate
- In Research Scientist, Data Engineer, DBA, Statistician and Other groups, professionals with 10+ years of experience are the biggest fraction of the users
- In Product/Project Management group, professionals with 5+ years of experience are the biggest fraction of the users
- In Business Analyst group, we see the users with 1-2 years of experience to dominate

### GSP Usage Patterns

We find that

- like for AWS, the top user groups for GCP are Data Scientists with 3-5 and 5-10 years of programming experience
- In Software Engineer, ML Engineer, and Data Analyst groups, professionals with  3-5 and 5-10 years of experience predominate (similar to GCP)
- In Research Scientist and DBA groups,  professionals with 10+ years of experience are the biggest fraction of the users
- In Data Engineer and Product/Project Manager groups, professionals with 3-5 years of experience predominate (as oppose to AWS)
- In Statistician and Other groups, junior-level professionals with 1-2 year of programming experience take the leadership

### MS Azure Usage Patterns

We find that 

- Data Scientists with 5-10 and 3-5 years of programming experience are the top user clusters for MS Azure
- Software Engineers and junior-level Business analysts are within the next tier of the users

## Usage of Cloud Service Providers: By Org Size/Data Science Team Size View

We are going to see how the top three cloud service providers (AWS, GCP, MS Azure) are used in the employer organizations where Kaggle survey responders work.

### AWS Usage Patterns

We find that AWS is mostly used by kagglers working in the organization types below

- Organizations with 0-49 employees, having 1-2 workers dedicated to Data Science workloads
- Organizations with 10000+ employees, having 20+ workers dedicated to Data Science workloads

### GCP Usage Patterns

We find that GCP is mostly used by kagglers working in the organization types below

- Organizations with 0-49 employees, having 1-2 workers dedicated to Data Science workloads
- Organizations with 10000+ employees, having 20+ workers dedicated to Data Science workloads
- Organizations with 0-49 employees, having 3-4 workers dedicated to Data Science workloads

So we can conclude that AWS and GCP tightly compete on the same types of the organizations/users.

### MS Azure Usage Patterns

We find that MS Azure is mostly used by kagglers working in the organization types below

- Organizations with 0-49 employees, having 1-2 workers dedicated to Data Science workloads
- Organizations with 10000+ employees, having 20+ workers dedicated to Data Science workloads

So we can conclude that MS Azure tightly ccompetes with AWS and GCP on the same types of the organizations/users.

## Usage of Cloud Computing Products

We find that 

- in the segment of cloud computing engines, Amazon EC2 is more popular than its rivals from Google (Google Cloud Computing Engine) and MS Azure (Azure Cloud Services)
- in the segment of cloud functions, AWS Lambda is more popular than its rivals from Google (Google Cloud Functions) and MS Azure (Azure Functions)
- in the segment of cloud container runners, Amazon Elastic Container Service is more popular that its rivals from Google (Google Cloud Run) and MS Azure (MS Azure Container Instances)
- Google holds the second place in cloud computing engine and cloud function segments, and it is on the third place in the cloud container runner segment
- there is a huge pool of responses with 'None', and it is most likely to indicate the entire market of cloud computing applications is not saturated yet

In terms of user roles, the most users of every cloud computing product above hold the roles below (top to bottom)
- Data Scientists
- Software Engineers
- ML Engineers
- Data Analysts

### Usage of Cloud Computing Products by Programming Experience

In addition to the insights above, we see that the top number of cloud computing product users fall into the following clusters in terms of their programming experience

- 5-10 years of experience
- 3-5 years of experience
- 10-20 years of experience

Juniors and super-seniors (20+ years of programming experience) seem to be less covered by the respective knowledge/skills.

## Usage of Cloud ML Products

We find that 

- Google Cloud AI Platform / Google Cloud ML Engine leads the ML cloud products usage 'nomination
- the second and third best are Amazon SageMaker and Azure Machine Learning Studio, respectively
- Data Scientists are the top users of cloud ML products (for every product investigated)
- There is a huge chunk of responders who indicated they do not use cloud ML products at all - this indicates the market is under-saturated, and there is a good growth potential, subject to resolving the marketing and end-user barries on the way

## Usage of Cloud ML Products by Programming Experience

In addition to the insights above, we can see that the cloud ML products are mostly used by the responders who has programming experience of

- 3-5 years
- 5-10 years

## Usage of Cloud ML Products by Organization Size and DS Capacity

We find that the majority of organizations in every size category does not use any Cloud ML Products at the moment.

For the tiny fraction of those who use them, there are interesting insights as follows

- in small organizations (0-49 employees), Google Cloud AI Platform / Google Cloud ML Engine dominates
- in the middle-sized organizations (50-249 employees), Google Cloud AI Platform / Google Cloud ML Engine and Amazon SageMaker titly
- for companies of bigger size (250+ employees), the size of Data Science team is often correlated with the preferred Cloud ML Product (smaller teams sticks to Google Cloud AI Platform / Google Cloud ML Engine more, and Data Science teams with 20+ headcount are more inclined to use Amazon SageMaker )

## Usage of Big Data Products By Occupation

We find that

- Overall top 3 list is constituted by three relational DBMS platforms (MySQL, PostgreSQL, MS SQL Server)
- MongoDB, a non-relational database platform, takes position 4 in the list
- Other relational DBMS platforms in the list (Oracle, IBM DB2, SQLite) are behind MongoDB
- In the segment of truly cloud-based Big Data products, Google BigQuery overruns its Amazon and MS Azure competitors (     Amazon Redshift, Amazon Athena, Amazon DynamoDB, and Microsoft Azure Data Lake Storage)
- Google Cloud SQL instances are still less popular then 'native' relational database instances for MySQL and PostgreSQL
- MS Access is still in use in the industry
- Data Scientists are the top users of each product in this list

## Big Data Product Usage Patterns by User Occupation and Programming Experience

We find that

- MySQL and PostreSQL are the  most popular database management platforms within each occupation
- MongoDB is quite popular with Software Engineers (although less popular then MySQL and PostreSQL)

## Big Data Product Usage Patterns by Organization Size and Data Science Capacity

We find that 

- Almost all of organizations except from the extra-large ones address their data management needs with MySQL, PostgreSQL, and MongoDB the most
- Extra-large organizations (with 10000+ employees) prefer to work with MySQL, MS SQL Server, Oracle, and PostgreSQL

## Usage of BI Tools

We find that

- Tableue and MS Power BI outperforms other rivals significantly
- Google Data Studio becomes a challenger to the leading BI products above, occupying the third place in the list
- Data Scientists, Data Analysts, Research Scientists, and ML Engineers are the most frequent users of BI tools
- Huge fraction of the survey responders indicated they do not use BI tools at all

## AWS Professional Users Across the Globe

We find that

- AWS is popular among survey respondents in India and USA the most
- Brasil, Japan and UK go into tier 2 in terms of the number of respondents from these country who use AWS

## GCP Professional Users Across the Globe

We find that

- India is the top country where GCP is used
- USA takes the second place in the rank but it is significantly below India (unlike AWS, where India and USA were relatively on a par)
- Japan and Brazil are in the tier 2 in terms of the number of respondents from these country who use AWS
- GCP is less popular in UK, Canada and Australia vs. AWS
- GCP outperforms AWS in Turkey, Indonesia, and Russia

## MS Azure Professional Users Across the Globe

We find that

- Top country in terms of the number of MS Azure users is India (although MS Azure is well behind AWS and GCP there)
- USA holds the second place in the rank, and the number of MS Azure users is on a par with the number of GCP users in the US
- Brazil belongs to tier 2 in term of the number of MS Azure users
- In the majority of the countries (except the US), the number of MS Azure users is smaller then the number of GCP and AWS users

# Chapter 5: Data Science Automation Tools

In this chapter, we are going to analize preferences of kagglers as for

- using automated machine learning tools
- using tools to help manage machine learning experiments

## Using Auto ML Tools: By-Purpose View

We find that

- the vast majority of the survey participants do not use any Auto ML tools in their daily routines
- automated model selection tools is the most popular type of Auto ML tools used by the kagglers at the moment
- automation tools for selecting a neural network architecture  are not vibrant and well known
- Data Scientists are the primary users of Auto ML tools (if in use)

## Using Auto ML Tools By Purpose and Size of Employer Organization

We find that

- Both the large-sized and small-sized organizations are equally represented across the cluster of organizations where auto ML tools are not used at the moment
- for each type of auto ML tools, the most usage of them is observed in small-sized organizations (it is also correlated with the fact the majority of the survey respondents work for such organizations in fact)

## Using Auto ML Tools By Purpose and Size of Data Science Team in Organizations

- Both the organizations with large-sized and small-sized data science teams are represented across the cluster of organizations where auto ML tools are not used at the moment
- if auto ML tools used, the most use of them is observed in organizations where Data Science team has capacity of 1-2, 3-4, or 20+ workers

## Utilizing Auto ML Tools By Product and User Occupation

We find that

- a lot of respondents indicated they do not use any auto ML product at the moment
- top three leading auto ML product (in terms of the number of respondents using them) are Auto-Sklearn, Auto-Keras, and Google Cloud AutoML
- Data Scientists are the primary users of auto ML products
- the next tier of roles played by the users of auto ML products contains Software Engineers, Data Analysts, and Research Scientists

## Utilizing Auto ML Tools By Product and User Occupation

In addition to the insights above, we find that

- for every auto ML product surveyed, professionals with 1-2, 3-5, 5-10, and 10-20 years of programming experiences are equally represented among the users
- professionals with 20+ years of programming experience are less attached to using auto ML products

## Utilizing Auto ML Tools By Product, Size of Organization, and Data Science Team Capacity

We find that

- small-sized organizations (0-49 employees) have more inclination to play around Auto-Scikitlearn and Auto-Keras
- for larger-sized organization, the biggest cluster is always the subset of organizations that do not use any auto ML, regardless the size of their Data Science team

## Utilization of Tools to Manage DS Experiments: By-Product and User Occupation View

We find that

- the majority of the survey respondents do not use any tools to help to manage data science experiments (so the market for such tools is extensively under-saturated)
- TensorBoard is the leading tool in use at the moment
- Data Scientists, Software Engineers, and Data Analysts are the top occupations of the users of such tools

## Utilization of Tools to Manage DS Experiments: By-Product and User Programming Experience View

In addition to the insights above, we find that

- the  users with 1+ year experience and more are equally represented in the pool of users of each helper product investigated

# Chapter 6: Knowledge and Information Sharing Channels

Knowledge is power, as Sir Francis Bacon told one day. Additionally, information becomes the power and 'new oil' in the modern post-industrial age.

Therefore it is essentially interesting to draw insights on how kagglers work with information as well as share/obtain professional knowledge.

In this chapter, we are going to analize the preferences of the survey participants as for

- platforms and tools to publicly share or deploy their data analysis or machine learning applications
- platforms to take online data science courses
- primary tools they use to analyze data
- favorite media sources that report on data science topics

## Public Sharing Platform Preferences by Occupation

We find that

- GitHub is the primary choice for Kagglers to share their work publicly
- Kaggle itself as well as Colab take the next places in the top 3 list of platforms to publicly share the work assets
- Good work sharing instruments like Streamlit and Plotly Dash are under-utilized by the community
- Quite a big fraction of the survey respondents indicated they do not share any work publicly
- The percentage of Business Analysts and people with 'Other' occupation who do not share their work results publicly is higher vs. the rest of the occupations

## Public Sharing Platform Preferences by Occupation and Programming Experience

In addition to the insights above, we find that

- GitHub and Kaggle are the preferred sharing platforms for every occupation and programming experience level groups
- The percentage of professionals not sharing their work results publicly is higher with more experienced professional groups (people with 10-20 and 20+ years of programming experience) - the replied with 'None' more frequently then other experience level group members

As my subjective opinion driven by the data insights above, Kaggle as a platform has an opportunity to involve the 'golden pool' of  experts (people with 10-20 and 20+ years of programming experience) to share their knowledge and wisdom with younter generations more actively if they 'crack the code' to motivate such professionals properly.

## Kaggle vs. Colab Usage

We can see that

- Kaggle is used more actively by males in the majority of occupations, levels of education and programming experience levels
- The most tangible diff is observed for male Data Scientists with Master's and Bachelor's degree, with programming experience between 1 and 10 years
- in a sense, we can think of Kaggle notebooks and Colab to compete over the same target audience

In the evidence of the above-mentioned data-driven insights, we can assume Google could benefit from re-positioning Colab from the functional and marketing stand-points, to drive more paying users to it.

## Online Training Platform Preferences by Occupation

We find that

- Coursera, Kaggle Learn Courses, and Udemy are in the top 3 list of preferred learning platforms (with Coursera being far more popular then the rest of the platforms in top 3 list)
- University courses leading to a formal university degree are also quite popular (it takes the 4th rank in the list)
- edX is behind its primary e-learning platform rivals
- only a minor fraction of respondents indicate they did not begin or complete data science courses (this is the healthy indicator of the data science community here at Kaggle to have good learning and self-learning attitudes)

## Online Learning Platform Preferences by Occupation and Programming Experience

In addition to the insights above, we find that

- Coursera is the top platform of choice by every occupation and programming experience level groups
- Kaggle Learn Courses are more popular with the inexperienced junior professionals (have <1 or 1-2 year of professional experience)
- For more senior professionals (with experience level of 3+ years), Udemy is the second platform of choice (after Coursera), and they do not actively use Kaggle Learn Courses

## Primary Data Analysis Tool Preferences by Occupation

We find that

- Local IDEs is the primary choice of the majority of the survey respondents (it highlights quite good technical skills of the respective respondents)
- Basic Stas software is the second preference of the respondents
- Data Scientists do not often use Basic Stas software as opposed to other analysis tool options investigated
- The rest of tool types goes far behind Local IDEs and Basic Stas software 

## Primary Data Analysis Tool Preferences by Occupation and Programming Experience

We can find that

- technically savvy occupations are more inclined to use Local IDEs as their primary 'data analysis' tool of choice whereas less technical occupations (like Business Analysts) tend to use basic stat tools more
- it is also noted that professionals with little programming experience (<1 year or zero experience) tend to choose basic stats softare whereas professionals with 2+ years of programming experience do not feel any fear of using local IDEs to serve their data analysis needs

## Favorite Media Sources by Occupation

We find that

- Kaggle as a medium of a valuable Data Science-related information it the top choice with the majority of the survey respondents, and it strongly out-performs other media sources investigated
- The second best is Youtube content
- Popular Data Science blogs take the third place in the rank
- other media sources are well below the top three media listed above

## Favorite Media Sources by Occupation and Programming Experience

In addition to insights above, we find that

- Almost in every occupation, people with programming experience of less then 10 years are funs of Kaggle as the primary information source
- People with 10+ years of experience tend to rank other information sources as s their primary  go-to medium choice Blogs a
- Junior Business Analysts (with 2 or less years of programming experience) rank YouTube as their primary go-to medium whereas more senior-level Business Analysts prefer Blog posts and Kaggle
- Statisticians with 20+ years of experience prefer Journal papers/publications, and Statisticians with less years of programming experience look the information up in Blogs and Kaggle as their go-to choices
- Product/Project managers rank Kaggle as their go-to information source, regardless their programming experience