# New-South-Wales-Remote-Working-Survey-Analysis

This data set is the result of surveying 1,500 employees in New South Wales, Australia. The survey was administered in late 2020 and again in 2021 with the intention of capturing attitudes to remote working in relation to COVID-19.

I've wanted to explore this data set for quite a while. This year I decided to learn data analysis with Excel and after a few smaller projects to get started, I decided to use Excel for this data set. I was interested in one thing and one thing only - did employees want to work fully remotely or not?

Knowing what I wanted to find out, I looked at the data. Questions were asked of respondents to obtain demographic and household information as well as employment information such as current industry, length of time in current role and size of current organization. The questions that interested me were three in particular:
  how much time was spent working remotely in 2021,
  how much time would respondents have preferred to work remotely in 2021, and
  how much time would respondents prefer to work remotely if COVID-19 was completely eradicated.
  
First up was data cleaning. For the purposes of presentation, the survey results needed to be modified. As they were, respondents had to choose between the following responses to each question, respectively:
  Rarely or never/I would not have preferred to work remotely/I would not prefer to work remotely
  Less than 10% of my time
  10%
  20%
  30%
  40%
  50% - I spent about half of my time remote working/50% - About half of my time/50% - About half of my time
  60%
  70%
  80%
  90%
  100% - I spent all of my time remote working/100% - All of my time/100% - All of my time

In order to have all responses be numerical, I used the IFS function to convert them to the following:
  0
  1
  10
  20
  30
  40
  50 
  60
  70
  80
  90
  100
 
 Next, I wanted to lay out the data so that I could compare these results, seeing how they were affected by the following factors:
  what industry respondents worked in,
  whether respondents lived in the metro area versus regional,
  how long respondents had been in their current job, and
  how many people were employed by their organization.
  
I thought PivotTables would be perfect for this as I could then create charts from the data and use slicers to filter the results. What I found was that I was able to do this for each question of interest withouth much issue. What I ideally wanted, however, was to look at the responses to each question in comparison to each other. The closest I could get to this in Excel on a Mac was by copying each PivotTable to a regular table and the using XLOOKUP to join them together, then creating a summary PivotTable out of that.

<img width="573" alt="image" src="https://user-images.githubusercontent.com/102552140/222872588-41a01fcc-613a-4b41-b0e3-5be64ad94f72.png">

Here is where I got stuck. I coudldn't go any further in Excel on my Mac, so I turned to Tableau Public hoping I could reach my desired destination. I got pretty close.

I remade the charts I had made in Excel and added the slicers, called filters in Tableau, connecting them to all three charts. I couldn't get the charts to merge into one, but I could put them alongside each other. That gave me the following.

![Dashboard 2](https://user-images.githubusercontent.com/102552140/222872749-4b223000-c8f1-482b-8926-55161d6f7f88.png)
