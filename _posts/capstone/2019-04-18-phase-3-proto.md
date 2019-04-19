---
layout: post
title:  "Prototype: Phase 3"
date:   2019-04-18 4:38:53 -0600
categories: [ Capstone ]
---

# Collaborative Music Machine

The *Collaborative Music Machine* (CMM) allows for multiple users to play music together from separate computers in the browser. Each user is assigned a color which corresponds to a set of UI controls. Users can only trigger actions on controls that are assigned to them. All controls, regardless of assignment, are always visible to all users. Users may suggest actions by interacting with controls that are assigned to another user. The user interface will indicate that a suggestion was made but no action will be triggered on the control unless it is acted on by the assigned user. 

Some other ideas to consider:

- Users can only make suggestions once they've acquired seniority. Seniority may be acquired over time or by other means.
- Users with higher seniority can trigger stronger suggestion indicators.
- Following a suggestion increases the seniority of the user who made the suggestion.
- Users can encourage other users through emotive actions (maybe emojis). Encouraging or discouraging a user may affect their seniority.
- Some controls may require multiple users to take action.
- Some controls may require a certain combined seniority to take action.
- Seniority may affect how many or which controls are available to a user.
- Controls begin unassigned and are assigned on a first come first served basis.
- Users may request or release ownership of controls to other users.
- As more people join, controls get split into smaller groups.
- Controls may become available over time.
- Users can write sequences and pass them to other users.

On how to separate controls, there are a few options:

- Each user is responsible for their own instrument and any related sequencing.
- Some users control instruments and some control sequencing.
- Some users make a selection of notes and other users sequence the notes.
- Each individual control is assigned randomly or on a first come, first served basis.
- Users are responsible for each of the same control across different instruments (e.g. all the levels, filter cutoffs, envelopes).

## Possible Synth UI Layout

<img src="{{ site.baseurl }}/assets/image/capstone-1/synth-layout.png" alt="screenshot" style="width:800px;"/>

The control set is inspired by FL Studio's 3xOsc. The synth includes 3 oscillators, each with level and pitch controls. All three oscillators are routed through amp, filter modules. The amp and filter can be modulated by the envelope which includes attack and release times. Finally, it as FX sends which correspond to global effects which are not shown. I used the 3xOsc with only my chosen controls to create some nice sounding presets. 

Here are some sounds I recorded with 3xOsc and random arpeggiators.
<iframe width="100%" height="265" src="https://clyp.it/0yygqj04/widget" frameborder="0"></iframe>

<img src="{{ site.baseurl }}/assets/image/capstone-1/3xosc.png" alt="screenshot" style="width:800px;"/>
