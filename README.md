# Intro to Coding for the Sports industry workshop at Birkbeck, University of London on 28/9/22
**Published Workshop event description is available [here](https://www.bbk.ac.uk/events/remote_event_view?id=33350).**
    
**Click on the link below to access the custom jupyterlite as the computational environment alongside the workshop code notebooks and data, or copy https://sportspython.github.io/BirkbeckSep22 into an appropriate browser:**
[![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://sportspython.github.io/BirkbeckSep22)
    
---

        
           
## Device Compatibility
* In theory, the custom jupyterlite should work on any device which meets the Browser Requirements, i.e. including tablets and mobiles. A laptop or desktop, where possible, is recommended however, for both performance and user experience.

## Browser Requirements

JupyterLite requires one of the following modern web browsers:

- Firefox 90+
- Chromium 89+

Use the normal window, i.e. `New Window` not a `New Private Window` or other anonymous window (known performance issues e.g. https://github.com/jupyterlite/jupyterlite/issues/679).

## Jupyter Requirements

%matplotlib inline needed to display matplotlib graphs in the jupyter notebooks.

## Some recommended keyboard Shortcuts for working in a Jupyter Notebook
(Note: you are expected to know how to/be able to upskill yourself to be able to operate a Jupyter Notebook and JupyterLab environment)    
* Use shift+enter to run code cells
* Use tab for auto-completion options
* Try shift+tab whilst writing a function to bring up it's documentation


## Sporting Context
* The Football Analytics content is based on the 21/22 English Premier League match between Arsenal and Man U on 23/4/22, at the time seen as a battle for 4th/the final Champion's League spot. The BBC's match report can be found [here](https://www.bbc.co.uk/sport/football/61125048).    
* The Sports Marketing content illustrates examples of Social Listening on Twitter for business insights into e.g. individual athletes, teams, brands etc., in this case centered on England Women midfield Keira Walsh's transfer from Man City to Barcelona in Sep '22.


## Documentation of the `match_events.csv` data

* The dataset coordinates are based on a 2D pitch positioned landscape with length 105 units (x-axis) by height 68 units (y-axis), and a coordinate system where (0,0) is bottom-right. The data shows Arsenal and Man U events as if they were attacking opposite goals, and attacking these same goals for the whole match/i.e. no change between the two halves. Arsenal data reflects them attacking the goal to the right i.e. at 105 units/maximum of the x-axis, with Man U data conversely reflecting them attacking the goal to the left, i.e. at 0 units/minimum of the x-axis. This is for consistency across both halves of the match to remove the need to re-calculate coordinates to account for a team's change of ends. You may still want to align the coordinates for both teams for adjusting one team's data by replacing it with the inverse values, for example if wanting to compare positions between the two teams' attacks on goal etc.

* The version of the match data, `match_events.csv`, is designed for introductory analysis focused on pass events, both completed and incomplete. As such, other events not in focus and/or would require less beginner-friendly workflows have been simplified or removed entirely, for example the records of set-piece events (kick-off, free kicks etc.).
