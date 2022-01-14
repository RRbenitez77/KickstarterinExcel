# Excel: Kickstart My Chart


![Kickstarter Table](Images/FullTable.png)

Excel was the tool used in this project where 4,000 Kickstarter projects that needed to be cleaned and narrowed down.Conditional formated cells in the 'State' column with identifiedd colors associated with Green for "Success or Red for "Failed" or canceled and currently "Live" campaign.The Excel spread sheet was extended to include another column 'percent funded' with a three-color scale from "red,"green" and "blue" additional Columns 'Average donation',sub-category' were added as well. Created a new sheet with stacked column piviot table to display the successful campaigns.





  ![Category Stats](Images/CategoryStats.png)


* The dates stored within the `deadline` and `launched_at` columns use Unix timestamps. Fortunately for us, [there is a formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) that can be used to convert these timestamps to a normal date.

  * Create a new column named `Date Created Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `launched_at` into Excel's date format.

  * Create a new column named `Date Ended Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `deadline` into Excel's date format.

  ![Outcomes Based on Launch Date](Images/LaunchDateOutcomes.png)

  * Create a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  * Now create a pivot chart line graph that visualizes this new table.

* Create a report in Microsoft Word and answer the following questions.

1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create?

## Bonus

* Create a new sheet with 8 columns:

  * `Goal`
  * `Number Successful`
  * `Number Failed`
  * `Number Canceled`
  * `Total Projects`
  * `Percentage Successful`
  * `Percentage Failed`
  * `Percentage Canceled`

* In the `Goal` column, create 12 rows with the following headers:

  * Less than 1000
  * 1000 to 4999
  * 5000 to 9999
  * 10000 to 14999
  * 15000 to 19999
  * 20000 to 24999
  * 25000 to 29999
  * 30000 to 34999
  * 35000 to 39999
  * 40000 to 44999
  * 45000 to 49999
  * Greater than or equal to 50000

  ![Goal Outcomes](Images/GoalOutcomes.png)

* Using the `COUNTIFS()` formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

* Add up each of the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.

* Create a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

## Bonus Statistical Analysis

If one were to describe a successful crowdfunding campaign, most people would use the number of campaign backers as a metric of success. One of the most efficient ways that data scientists characterize a quantitative metric, such as the number of campaign backers, is by creating a summary statistics table.

For those looking for an additional challenge, you will evaluate the number of backers of successful and unsuccessful campaigns by creating **your own** summary statistics table.

* Create a new worksheet in your workbook, and create a column each for the number of backers of successful campaigns and unsuccessful campaigns.

  ![Images/backers01.png](Images/backers01.png)

* Use Excel to evaluate the following for successful campaigns, and then for unsuccessful campaigns:

  * The mean number of backers.

  * The median number of backers.

  * The minimum number of backers.

  * The maximum number of backers.

  * The variance of the number of backers.

  * The standard deviation of the number of backers.

* Use your data to determine whether the mean or the median summarizes the data more meaningfully.

* Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?

## Submission

* To submit your homework, upload the solution and files to a GitHub repo, Dropbox, or Google Drive and submit the link to <https://bootcampspot.com/>.

## Employer-Ready Criteria

Students who are marked as employer-ready gain access to our employer referral program, additional workshops, and other resources. Work with your Career Director to become employer-ready. At a minimum, you must have:

- A clear, concise, and compelling resume. Submit via your learning platform for review.
- A polished GitHub profile:
  - 3 - 6 pinned repositories ([instructions here](https://docs.github.com/en/enterprise/2.13/user/articles/pinning-items-to-your-profile))
  - at least 5 commits per repository
  - professional titles, i.e. not "Homework #1"
  - thorough README.md files for each repository
  - clean code

- - -
Given the provided data, what are the three conclusions we can draw from the Kickstarter Campaigns?

A: Successful campaigns significantly decline during Nov/Dec possibly attributed to Holliday spending. The successful campaigns dip past failed campaigns.


What are the limitations of the Dataset?

A: Not much is known about the relationship between backers and campaigns this could help potentially highlight if campaigns are being self-funded to start with to get momentum, then they are backed by others that have interest thereafter.

What are some other possible tables & Graphs that we could create?

A line graph where the x axis states the campaign timeline from Live through successful funding ,canceled and Failed and on the Y- axis the amount that was contributed to visualize how soon or how long it should take to be successful or be a failure.
![image](https://user-images.githubusercontent.com/33403205/149434118-ff9b4c2a-677e-402e-abf8-452d34606af3.png)
