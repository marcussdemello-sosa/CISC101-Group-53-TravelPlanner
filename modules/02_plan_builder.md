Change Log (2025-11-13):
- Added a rule to add a short break on long days to ensure realistic pacing.

Create a short list of candidate activities (e.g., attractions, restaurants, parks).  
Each activity includes type, estimated duration, cost range, and distance.

Use a simple loop to build days:

for each day:  
    pick Morning activity (near lodging)  
    pick Midday activity (close by)  
    pick Afternoon activity (different theme)  
    pick Evening restaurant or optional event

New rule: If day is long (3+ hours before evening), add a short break between noon and evening automatically. 
