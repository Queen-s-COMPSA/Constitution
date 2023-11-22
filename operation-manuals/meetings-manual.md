---
title: Meetings Operations Manual
subtitle: Queen's Computing Students' Association
date: November 2023
---

# Meetings

Meetings are critical to ensuring there is strong communication within
COMPSA; making sure everyone is on the same page.

Governance & Culture is responsible for scheduling and managing all COMPSA-wide
meetings.

There are three recurring compsa-wide meetings that happen throughout the year:

| interval      | Meeting               |
|---------------|-----------------------|
| every 3 weeks | General Assembly (GA) |
| biweekly      | Council Meeting       |
| biweekly      | All Hands Meeting     |

One of these meetings happens Each week. General Assemblies & All Hands
Meetings happen every 4 weeks; Council Meetings happen every 2 weeks. 

## Schedule

These meetings are scheduled on a four week interval, each happening
consecutively and on the the same day of the week

| Week | Meeting           |
|------|-------------------|
| 0    | General Assembly  |
| 1    | Council Meeting   |
| 2    | All Hands Meeting |
| 3    | Council Meeting   |

Additionally, the Meetings should begin at the start of the year as follows:

| Meeting          | Start                                    |
|------------------|------------------------------------------|
| All Hands        | Monday before first GA                   |
| General Assembly | First possible Monday of the school year |

And after this, the 

Consider the sequence diagram (because compsci) illustrating the meeting
schedule interval:

```mermaid
stateDiagram-v2

GA : General Assembly
CM : Council Meeting
AH : All Hands Meeting

state startOfYear{
    FAH : First All Hands
    FGA : First General Assembly
}

FAH --> FGA : First possible monday of the school year
FGA --> CM : First Monday after GA

GA --> CM : First Monday after GA
CM --> AH : Second Monday after GA
AH --> CM : Third Monday after GA
CM --> GA : Fourth Monday after GA
```

Note: In the past, Monday; 5-6, in Walter Light 210 and the COMPSA Office has
worked well.

## General Assemblies

> General Assemblies are a time for all members of COMPSA (students in the
> school of Computing) can come and voice ther concerns about the current affairs
> of Computing Students.

General Assemblies (GAs) are held in a large classroom or auditorium, typically
in Goodwin or Walter-Light Halls.
During the GA, the speaker conducts the meeting following Burnoits Rules of
order (however, strictly following them is not necessary)

## Council Meetings

> Council Meetings are a time for Ministers and the Executive to update
> eachother on what they have been working on, and to plan & collaborate on future
> tasks

These meetings are normally held in the COMPSA Office. The start of the meeting
should consist of everyone giving updates on what they have done and what they
plan to do for the upcoming weeks. After this is done, executives should go into
groups with their portfolios to discuss things in a more dynamic way --
allowing ministers to collaborate with other directors.

## All Hands Meetings

> All Hands Meetings are a time for all members of COMPSA to mingle (attendance
> is mandatory) and for the Executive and Council to update working members of the
> goings-on at COMPSA.

The meeting should begin with _brief_ updates from the Exec and Council, and
should be followed by a small social for volunteer appreciation. 

While Governance & Culture handles organizing the meeting, it is traditional for the Exec to
manage the volunteer appreciation afterwards.