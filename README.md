<img width="856" height="688" alt="image" src="https://github.com/user-attachments/assets/30262200-4397-4a9c-8353-005b268d3675" />
<img width="3191" height="2373" alt="image" src="https://github.com/user-attachments/assets/5ce288c0-a1cb-4548-a335-2cf69bed0973" />
<img width="1373" height="584" alt="image" src="https://github.com/user-attachments/assets/29d7cd78-4006-4520-8a1a-0463ea6919cf" />


 COFFEE EXTRACTION ANALYSIS + RECOMMENDER ENGINE

About This Project

I've always been curious about how different coffee brewing methods actually compare—not just in taste, but in measurable things like caffeine content, acidity, and antioxidants. So I dug into the data on 13 brewing methods and built a recommender engine to help people find their perfect cup.

What I Wanted to Find Out

Which method gives you the biggest caffeine kick?
Does longer brewing time always mean more caffeine? (Spoiler: no)
What's the healthiest way to brew coffee?
How do acidity, bitterness, and body vary across methods?
Most importantly—which method fits your specific preferences?
The Data

I looked at 13 common brewing methods. Here's a sample:

Method	Time (min)	Caffeine (mg)	Antioxidant Rank	Acidity (1-10)	Bitterness (1-10)	Body (1-10)
Ristretto	0.37	127	4	5	8	9
Espresso	0.47	124	3	6	7	9
AeroPress	1.50	60	1	5	4	5
Moka Pot	4.00	548	3	4	6	8
Pour Over	4.50	173	2	8	3	4
French Press	4.50	186	3	4	6	8
Cold Brew	1080	560	2	2	2	6
13 methods total, including Turkish, Lungo, Chemex, etc.

What I Found

Here are the highlights:

Finding	Result
Strongest caffeine	Cold Brew (560mg) and Moka Pot (548mg) — almost identical
Fastest brew	Ristretto (22 seconds) and Espresso (28 seconds)
Most antioxidants	AeroPress took the top spot
Most acidic	Pour Over (8/10) — bright and tangy
Most bitter	Ristretto, Lungo, Turkish (all 8/10)
Fullest mouthfeel	Ristretto and Espresso (9/10) — syrupy and thick
The Most Interesting Thing I Learned

Brew time barely matters for caffeine.

I honestly expected cold brew to blow everything else out of the water since it steeps for 18 hours. But compared to espresso (28 seconds), it only has about 4.5 times more caffeine. That's not nothing, but it's way less dramatic than I thought. Something about extraction efficiency—espresso uses pressure and heat to pull caffeine out crazy fast.

Visualizations I Made

I created four main charts to make sense of the data:

Caffeine ranking — bar chart showing highest to lowest
Time vs caffeine — scatter plot with log scale (that's where you see the weak relationship)
Correlation heatmap — shows how different attributes relate to each other
Taste profile comparison — spider chart comparing methods side by side
All generated in Python using Matplotlib and Seaborn.

The Recommender Engine

This was the fun part. I built a system that asks you five questions and matches you with your top 3 brewing methods.

The Questions

Question	Your Options
How much time do you have?	Instant / Fast / Medium / Slow / Very Slow
What taste do you want?	Very Bright / Bright / Balanced / Bold / Very Bold
What's your goal?	Max energy / Quick boost / All-day sipping / Healthy / Light
What body do you prefer?	Light / Medium / Full / Very Full
Caffeine sensitivity?	Very sensitive / Moderate / High tolerance
How Scoring Works

Every brewing method starts at 0. For each answer you give, any method that fits that preference gets 1 point. Perfect match = 5 points. Then I rank them and show you the top 3.

For example, if you choose "Fast" + "Very Bold" + "Max energy" + "Full body" + "High tolerance" — you're probably getting Ristretto or Espresso as your top pick.

Interactive Dashboard

I put the whole thing into Tableau Public so you can actually use it interactively. You can filter by any attribute, compare methods visually, and run the recommender.

Live Dashboard:  [https://public.tableau.com/app/profile/brian.ma5935/viz/BrianCoffeeProject/Dashboard1](https://public.tableau.com/app/profile/brian.ma5935/viz/BrianCoffeeProject/Dashboard1) 

Github: [https://github.com/brianphu2310/COFFEE-EXTRACTION
](https://github.com/brianphu2310/COFFEE-EXTRACTION)

Tools I Used

Tool	What I Used It For
Excel	Storing and cleaning the initial data
Python (Google Colab)	Analysis, stats, and generating all the charts
Tableau Public	Building the interactive dashboard and recommender
Want to Try It Yourself?

The data and code are all here. You can:

Run the analysis notebook in Colab
Recreate the charts with your own data
Tweak the recommender scoring system
Add more brewing methods
A Couple Limitations

A few things I'd do differently next time:

Antioxidant ranking was qualitative (1-4 scale) — lab measurements would be better
Caffeine varies by bean and roast, so these are averages
"Body" and bitterness are subjective — I used consensus from specialty coffee sources
But for a practical guide to choosing a brewing method? It works pretty well.
