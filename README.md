# Trump Truth Social
This is a CSV file containing "truths" scraped from the Truth Social Social Media Service. The data collection was performed on October 14th, 2025. Note, 
1) Contains truths from the inception of Trump's account in Feb. of 2022 - Oct 14th 2025
2) Time is in EST
3) Only contains truths containing text. Media (i.e, photo and video) truths were not collected.
4) Data was collected using TruthBrush 


# Trump Market Truths
This CSV was constructed from the full CSV, but specifically has been limited to the subset of truths posted between stock market hours of (9:30am-4:00pm), during the time of Trumps Presidency. 
It was adapted (but not fully finished) to the current research question. It has an indicator column for holidays, which the market is closed or closes early. 
RQ: Do Trump's posts on TruthSocial during market hours provide explanatory value on the response variable of SPY price fluctuation on different time scales? 

# Trump Open Market Truths
This CSV is constructed from the TMT Csv, but has specifically limited weekends as well as all holidays. Testing on this csv has shown 100% call rate success with the polygon API. 

# Performance Table
This CSV went through all of the non-weekend posts made by Donald Trump between market hours since his presidency in 2025, and checked the performance of the Polygon API to collect the ticker price candle at the desired time. 
Our performance table most importantly showed us that it was able to grab the price candle at the desired timestamp for everything except the errors, which were dueto  holidays, which we expected to happen. It didn't error on all of the market holidays we took into account, and this is because some holidays only had the market closed for a portion of the day rather than the full day and the post was likely made on the holiday while market hours were still in session, For example on July 3rd before 1pm. For simplicitiy, we are going not to consider holidays at all, even the select few which didn't have errors, since we don't believe they generalize well for typical non-holiday market conditions.  

# Performance Errors 
Due to holidays. 
