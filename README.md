# Power BI Project: Sports by Skills Rating

## Project Overview
This Power BI project analyzes 60 sports based on 10 different skills that are crucial to athletic performance. The data is sourced from ESPN and rates each sport’s reliance on skills such as endurance, strength, power, speed, agility, flexibility, nerve, durability, hand-eye coordination, and analytic aptitude on a scale from 1 to 10.

The report allows users to explore how each sport ranks across various skill sets, providing insightful comparisons and enabling sports enthusiasts, coaches, and analysts to better understand the physical and mental demands of each sport.

---

## Sports Covered (60)
Boxing, Ice Hockey, Football, Basketball, Wrestling, Martial Arts, Tennis, Gymnastics, Baseball/Softball, Soccer, Alpine Skiing, Water Polo, Rugby, Lacrosse, Steer Wrestling, Pole Vault, Field Hockey, Speed Skating, Figure Skating, Distance Cycling, Volleyball, Racquetball/Squash, Surfing, Fencing, Freestyle Skiing, Team Handball, Sprint Cycling, Bobsledding/Luge, Ski Jumping, Badminton, Nordic Skiing, Auto Racing, High Jump, Long/Triple Jumps, Diving, Distance Swimming, Skateboarding, Sprint Track Events, Rowing, Calf Roping, Distance Track Events, Bull/Bareback Riding, Middle Distance, Weightlifting, Sprint Swimming, Water Skiing, Table Tennis, Track Weights, Canoe/Kayak, Horse Racing, Golf, Cheerleading, Roller Skating, Equestrian, Archery, Curling, Bowling, Shooting, Billiards, Fishing.

---

## Skills Rated (10)
- **Endurance:** Ability to perform continuously for long periods (e.g., Lance Armstrong).  
- **Strength:** Ability to produce force (e.g., NFL linebackers).  
- **Power:** Ability to exert force quickly (e.g., Barry Bonds).  
- **Speed:** Ability to move rapidly (e.g., Marion Jones).  
- **Agility:** Ability to change direction quickly (e.g., Derek Jeter).  
- **Flexibility:** Range of motion in joints (e.g., gymnasts).  
- **Nerve:** Overcoming fear (e.g., race-car drivers).  
- **Durability:** Withstand physical strain (e.g., NBA players).  
- **Hand-Eye Coordination:** Reacting quickly to sensory cues (e.g., baseball hitters).  
- **Analytic Aptitude:** Strategy evaluation and reaction (e.g., quarterbacks).

---

## Data Transformation Process
1. Imported the Excel file into Power BI.  
2. Selected the relevant sheet and opened Power Query.  
3. Unpivoted the skill columns (10 skills), leaving `Rank` and `Total` untouched.  
4. Created two columns:  
   - `Skills`: lists each skill type for every sport  
   - `Skill value`: the rating (1–10 scale) for that skill in the sport  
5. Merged `Rank` and `Sport` into a single column named **`Sport slicer`** using ‘-’ as a separator (e.g., `1-Boxing`).  
6. Final columns:  
   - `Rank`  
   - `Skill value`  
   - `Skills`  
   - `Sport`  
   - `Total`  
   - `Sport slicer`  
7. Applied "Close & Apply" to load the data.

---

## Report Design
The report is divided into three sections:
1. **Header:** Contains the title and styling elements.  
2. **Slicers:** Interactive filters allowing users to select sports.  
3. **Main Area:** Visuals and insights.

### Key Features
- Imported **Chiclet Slicer** from the Power BI marketplace.  
  - Used `Sport slicer` as the field.  
  - Set layout to 12 columns to accommodate all 60 sports.  
  - Sorted by `Rank` for serial ordering.  
  - Disabled multi-select for logical consistency.
  
- **Stacked Bar Chart:**  
  - X-axis → `Skill value`  
  - Y-axis → `Skills`

- **Text Description:**  
  - Added explanations of each skill in a blank area for user understanding.

- Applied a consistent theme and background across the report and separated sections with lines for clarity.

---

## Tools Used
- **Microsoft Power BI**  
- **Power Query** for data transformation  
- **Chiclet Slicer** for enhanced interactivity  

---

## Final Deliverables
An interactive and visually engaging report that allows users to:
- Compare how different sports demand specific skills.  
- Filter by sport for detailed exploration.  
- Analyze sports performance requirements on a scale of 1 to 10.

This project offers a unique perspective on the athletic demands across a wide variety of sports and helps users gain deeper insights into the underlying attributes that drive performance.

---


