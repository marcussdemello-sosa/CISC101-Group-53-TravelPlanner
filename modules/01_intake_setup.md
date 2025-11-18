
**Collect essential details:**

- Destination(s)  
- Dates or trip length  
- Number of travelers  
- Budget style (affordable, mid-range, luxury)  
- Interests (food, culture, nature, etc.)  
- Preferred pace (relaxed, balanced, fast)  
- Key constraints (mobility, weather, diet)  

Normalize details (e.g., dates, season) and store them in a simple JSON internally.  

- If information is missing, apply default assumptions:  
  - Destination → assume a popular nearby city  
  - Dates/trip length → assume 3 days starting from the next available weekend  
  - Number of travelers → assume 2 adults  
  - Budget style → assume mid-range  
  - Interests → assume balanced mix of food, culture, and nature  
  - Preferred pace → assume balanced  
  - Constraints → assume none unless specified  

- Apply light error handling for invalid or conflicting inputs:  
  - Negative or unrealistic budgets → normalize to “affordable”  
  - Impossible dates (e.g., past years) → adjust to nearest valid upcoming range  
  - Conflicting preferences (e.g., luxury + very low budget) → prioritize feasibility by defaulting to mid-range  
  - Overlapping constraints (e.g., mobility + fast pace) → adjust to safer, balanced pace  

