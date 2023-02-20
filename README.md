# Income Inequality between CEOs and Workers, and Layoffs

![Wealth Inequality](images/p9-basu-a-20180416.jpg 'Wealth Inequality')
## Introduction

We start with two datasets. 

The first one compiles the S&P 500 companies with the CEO and the median worker salary. We compute the ratio between these two in order to describe the inequality. We also have listed down the industry to which they belong.

The second dataset collects all the published layoffs by technology companies in the past two years. We are also given the percentage of the company being layed off, as well as the headquarters location, public/private status, and specialization within tech.

As a final dataset, we attempt to merge the two datasets on their company names. Due to the nature of the datasets coming from different sources, we have to do a 'fuzzy' merge in order to account for differences in spelling and/or full names.

![Database Structure](images/erd.png 'Database Structure')

## The Beginning: CEO vs Worker Salary

We set our gaze upon the first page. Our first object of interest is the infobox at the top left. It contains the company with the biggest pay discrepancy between the CEO and the average worker. The largest in our dataset is a whopping 1:21125 ratio held by Nu Skin Enterprises. Using the slicer at the top we can scroll through all the industries in our data, and we can see the smallest industry gap is in the energy sector.

To put it into easier to visualize terms, we can focus on the pie chart describing the piece of the pie that the CEO takes home versus the average worker, with the latter's slice being barely visible.

Finally, our scatter graph plots all of our datapoints, which at first seems relatively reasonable, until we zoom into the axes units: one is in millions, and the other in hundreds of millions; two orders of magnitude difference.

## Next Page: Layoffs in the Tech Industry

![Layoff Heatmap](images/map.png 'Layoff Heatmap')

The main draw is the background. We see that the heat map only has any significant data in the United States of America. It is not surprising, since both the largest amount of tech companies are located there, but also due to their very lax labour laws.

The first two data points to take in are the number of jobs lost, as well as what the average of the percentages of the workforces in the company were lost.

On the right hand side, we have two graphs. The first is a simple time progression plot, exemplifying the sudden increase in layoffs in the post-pandemic economic cooldown in tech, peaking in early 2023. The second graph is slightly more interesting. We obtained the data sets by fuzzy-merging our two different datasets and we find the perhaps unsurprising weak positive trend that the companies that layed off the most employees also paid their CEOs a higher salary. Food for thought.

The pie chart gives a breakdown between type of company (public/private). The public companies had more layoffs overall per company, but there were significantly more private companies that had minor amounts of layoffs.

Finally, the bar chart explains the difference between specialization within the industry and jobs affected. Amazon, Microsoft and Cisco lead the SaaS category almost singlehandedly. There is some intersection between the former and the next largest category: E-Commerce. It is again quite predictable that this sector is one of the most affected, as post-pandemic spending relied less and less on web infrastructure as restrictions were lifted. Similarly for journalism, the third largest, fewer restrictions meant fewer reasons to spend more time reading articles online, and therefore declined.

## Conclusion

What can we take in from these?

It is not a positive outlook for industry as a whole. Tech is just one aspect of the global economy, but new tech developments are the most prone to creating bubbles in our current lifestyle, and the post pandemic decline exemplifies the disposability of labour, especially within the United States.

Many would like to argue that it is justified that CEOs are worth more to a company and therefore should have a comparatively larger salary to dignify their presence. While it is true in the private sector that they tend to be majority stakeholders and therefore incur disproportionately more risk, most of the layoffs happened in the public sector, where a CEO's short-term performance and profits are highly valued amongst the outsider stakeholders, with a common strategy to dispose of the workers to boost the end of quarter/year financial statements. There is no risk - only makeup.

Europe disencourages this practice simply by the fact that there are both more labour rights, as well as high financial cost to firing employees without a clear motive. Some argue that it encourages laziness and underperformance, since an employee can feel more secure in their job. On the other hand, one could argue that this security would positively impact their mental health and wellbeing, and therefore be more likely to produce better work per time spent. It would simultaneously implicitly force companies to look towards more long-term profit goals which introduces less volatility and a stronger backbone to their country's economy.

It is true that American companies have become the largest and most successful in the world, but at what cost? Is the American population in a better position thanks to them? Is destabilizing global economies, introducing systemic poverty and creating social divide for profits a positive for the world? Or just for the few stakeholders?
