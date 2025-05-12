---
{"dg-publish":true,"dg-path":"fragments/Maxwrites activity maps.md","permalink":"/fragments/maxwrites-activity-maps/","created":"2025-05-11T20:12:04.548-04:00","updated":"2025-05-11T20:16:48.565-04:00"}
---


# Maxwrites activity maps 
Contribution Graph Heat Map plugin showing usage over the last 6 months. This includes usage of the whole Obsidian vault, not just the digital garden.

```contributionGraph
title: Contributions
graphType: month-track
dateRangeValue: 6
dateRangeType: LATEST_MONTH
startOfWeek: 0
showCellRuleIndicators: true
titleStyle:
  textAlign: left
  fontSize: 15px
  fontWeight: normal
dataSource:
  type: PAGE
  value: ""
  dateField:
    type: FILE_MTIME
fillTheScreen: false
enableMainContainerShadow: false
cellStyle:
  borderRadius: 50%
cellStyleRules:
  - id: Halloween_a
    color: "#fdd577"
    min: 1
    max: 2
  - id: Halloween_b
    color: "#faaa53"
    min: 2
    max: 3
  - id: Halloween_c
    color: "#f07c44"
    min: 3
    max: 5
  - id: Halloween_d
    color: "#d94e49"
    min: 5
    max: 9999

```

