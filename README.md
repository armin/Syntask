# Syntask

> A simple syntax for lists and daily schedules, inspired by Markdown.

Syntask allows you to write a daily task list in plain text format, then convert it to structurally valid day schedule using a productivity apps such as the Prepd app.

Syntask is like Markdown but for time based things to quickly write daily schedules or step-by-step timelines. 

# Concept

Every line in Syntask text is a single thing in a list. There is an expectation that the text can be converted by apps into a schedule with start/end time for each activity. Start and end times are calculated based on time anchors and the duration of activities and sequence of activities. 

## Sample:
    __ Monday __
    7 am (time) 
    Breakfast (1)
    Commute (1)
    9 am (time) 
    Project A (2)
    Project B (2)
    12 pm (time)

An app that uses Syntask should display additional information that can be calculated such as free time in a time block or start and end time for activities.

## Monday

**7 am   (30m free)**

- Breakfast    1h
- Commute   30m

**9 am   (2h free)**

- Project A   1h
- Project B   1h

**12 pm** 


## Monday

**7 am**   

- Breakfast    7am - 8am (1h)
- Commute   8am - 9am (30m)

**9 am**  

- Project A   9am - 10am (1h)
- Project B   10am - 11am (1h)
- *Free 11am - 12pm* 

**12 pm** 

# Syntax
    Activity (1)
    Large Activity (epic)
    __ Divider __
    Block (block)
    Theme (theme)
    12 pm (time)


## Potential Syntax
    Free (filler)
    ( ) checklist item
    (x) checked checklist item
    (>) indented item

