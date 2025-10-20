---
title: Argentina's Unsung Hero
author: Toochukwu Ogbonna
date: '2025-01-26'
slug: []
categories:
  - football
tags:
  - football
  - worldcup
excerpt: A look into the role of Rodrigo De Paul in Argentina's triumph at the 2022 world cup in Qatar
---

------------------------------------------------------------------------

**When** you think of Argentina’s World Cup victory, a couple of things come to mind: Messi’s crowning moment, that Martinez save against Kolo Muani, Enzo Fernandez’s break into the world consciousness, Di Maria scoring in yet another final, Scaloni’s burst to the global scene and if you’re being a bit cynical, the five penalties Argentina had. Irrespective of what you think, there is a consensus that it was one of the most memorable World Cup tournaments, and it had one of the greatest football matches ever let alone a World Cup final culmination in what can only be regarded as the crowning moment in Messi’s illustrious career. What might not immediately come to mind, though, is the contribution of Rodrigo de Paul in that Argentina victory. Let’s explore the contributions of Argentina’s Unsung hero - Rodrigo De Paul

> <p style="font-style: italic";> "He was beautiful. He was the point of difference. He has always been the point of difference. Unparalleled, and maybe today, there will, of course, always be those who argue, always be those who debate. And the debate could rage on if you like. But as he falls in love with the object in the world that his heart most desired, it is hard to escape the supposition that he has rendered himself today, the greatest of all time"</p>

> — Peter Drury

**Availability**

We first consider his availability before exploring what made him especially important in the 20202 World Cup run. While injuries are common in any sport, and no player is immune or exempt from injury, every manager prays they can always field their best eleven in a seven-game competition. Rodrigo de Paul avails himself of this wish. He Started all seven games, completed three, and played a combined total of minutes. He was fourth in minutes played among Argentines behind Lionel Messi, Emi Martinez and Otamendi.

> “Availability is the best ability.”
>
> — Charles Barkley

<img src="{{< blogdown/postref >}}index_files/figure-html/plot of minutes played-1.png" width="672" style="display: block; margin: auto auto auto 0;" />

When he was substituted against the Dutch Argentina were already a goal up and were 3 goals up and when he was substitute against the Croats.

<img src="{{< blogdown/postref >}}index_files/figure-html/plot-of-matches-played-1.png" width="672" style="display: block; margin: auto auto auto 0;" />

**Centrality**

Graphs and networks are a good way to measure the influence of elements in a system, so we’ll explore just how important RDP was to this Argentine team. Before going into the finer details, we can see from the pass map how central Enzo was to the way the team was set up, both literally and figuratively; he made the teamwork, but we could argue that the RDP’s role was just as important if not more; he made Messi work. The gameplan seems simple enough, Molina to RDP to Messi, showing just how dependent Argentina was on that right-hand side; the fact that both Taglafico and Acuna, who are both left-backs, were among the top 10 outfield Argentine players with the most minutes and Di Maria, who also plays on the left side, isn’t among the shows just how reliant they were on the right side.

<div class="figure" style="text-align: left">

<img src="{{< blogdown/postref >}}index_files/figure-html/generating-passmap-1.png" alt="passmap" width="3600" />
<p class="caption">

<span id="fig:generating-passmap"></span>Figure 1: passmap
</p>

</div>

Using the graph networks show essentially the same thing as the pass map shows. What we can, however, do with the maps is that we can quantify just how important he was to the team as a whole

<div class="figure" style="text-align: left">

<img src="{{< blogdown/postref >}}index_files/figure-html/network-map-1.png" alt="Argentina Network Plot" width="1500" />
<p class="caption">

<span id="fig:network-map"></span>Figure 2: Argentina Network Plot
</p>

</div>

The node size corresponds to the number of passes given and received, and the thickness of the lines represents the number of passes given. This gives us a clearer picture of the player’s influence.

First, we examine some descriptive measures of network systems and then consider the player’s influence on the system in terms of the measures.
1. Degree centrality is the most straightforward and intuitive measure of centrality; it simply depends on the number of edges each node has. In the context of football and this data, it merely shows how many passes a player has received. Since we have passes made and passes received, measuring the IN (passes received) and OUT (passes given) Degrees is possible. The combination of both is just called the Degree. The Degree is equivalent to the player’s size, which is already represented in the pass map and the graph above.

2.  Betweenness Centrality measures how important nodes or players are to the flow of a network; a node or player with high Betweenness facilitates the movement of information or the ball in football. By calculating the shortest path between nodes, we can get betweenness centrality. The Betweenness of players in a game can demonstrate how a team plays; if the team prioritises passing it from the back and playing through the middle, we can expect its defenders and midfielders to have higher measures of Betweenness.

3.  Closeness centrality indicates how close a node is to another node in the network. It shows how close players are to each other in terms of receiving passes from other players.

4.  We measure the influence of the players in the network using the page rank and eigen centrality algorithms, while they are similar - the PageRank is based on the eigen- they are still different. Eigen depends on the number of connections a node has, and the number of connections each node it connect to also has iot rewards for nodes that have connections to highly connected nodes. Page rank differs from the Eigen in that it also accounts for the indegrees of the node, which the eigenvector does not.

<div id="ccrjavgnrr" style="padding-left:0px;padding-right:0px;padding-top:10px;padding-bottom:10px;overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>@import url("https://fonts.googleapis.com/css2?family=Chivo:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Chivo:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Chivo:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Cairo:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");
#ccrjavgnrr table {
  font-family: Cairo, system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
&#10;#ccrjavgnrr thead, #ccrjavgnrr tbody, #ccrjavgnrr tfoot, #ccrjavgnrr tr, #ccrjavgnrr td, #ccrjavgnrr th {
  border-style: none;
}
&#10;#ccrjavgnrr p {
  margin: 0;
  padding: 0;
}
&#10;#ccrjavgnrr .gt_table {
  display: table;
  border-collapse: collapse;
  line-height: normal;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: 400;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: none;
  border-top-width: 3px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_caption {
  padding-top: 4px;
  padding-bottom: 4px;
}
&#10;#ccrjavgnrr .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}
&#10;#ccrjavgnrr .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 3px;
  padding-bottom: 5px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}
&#10;#ccrjavgnrr .gt_heading {
  background-color: #FFFFFF;
  text-align: left;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_bottom_border {
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_col_headings {
  border-top-style: none;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #000000;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}
&#10;#ccrjavgnrr .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}
&#10;#ccrjavgnrr .gt_column_spanner_outer:first-child {
  padding-left: 0;
}
&#10;#ccrjavgnrr .gt_column_spanner_outer:last-child {
  padding-right: 0;
}
&#10;#ccrjavgnrr .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #000000;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}
&#10;#ccrjavgnrr .gt_spanner_row {
  border-bottom-style: hidden;
}
&#10;#ccrjavgnrr .gt_group_heading {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: none;
  border-top-width: 2px;
  border-top-color: #000000;
  border-bottom-style: solid;
  border-bottom-width: 1px;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  text-align: left;
}
&#10;#ccrjavgnrr .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: none;
  border-top-width: 2px;
  border-top-color: #000000;
  border-bottom-style: solid;
  border-bottom-width: 1px;
  border-bottom-color: #FFFFFF;
  vertical-align: middle;
}
&#10;#ccrjavgnrr .gt_from_md > :first-child {
  margin-top: 0;
}
&#10;#ccrjavgnrr .gt_from_md > :last-child {
  margin-bottom: 0;
}
&#10;#ccrjavgnrr .gt_row {
  padding-top: 3px;
  padding-bottom: 3px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}
&#10;#ccrjavgnrr .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 0px;
  border-right-color: #FFFFFF;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#ccrjavgnrr .gt_stub_row_group {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 5px;
  padding-right: 5px;
  vertical-align: top;
}
&#10;#ccrjavgnrr .gt_row_group_first td {
  border-top-width: 2px;
}
&#10;#ccrjavgnrr .gt_row_group_first th {
  border-top-width: 2px;
}
&#10;#ccrjavgnrr .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#ccrjavgnrr .gt_first_summary_row {
  border-top-style: solid;
  border-top-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_first_summary_row.thick {
  border-top-width: 2px;
}
&#10;#ccrjavgnrr .gt_last_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#ccrjavgnrr .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_last_grand_summary_row_top {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-bottom-style: double;
  border-bottom-width: 6px;
  border-bottom-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}
&#10;#ccrjavgnrr .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#ccrjavgnrr .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}
&#10;#ccrjavgnrr .gt_sourcenote {
  font-size: 12px;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 5px;
  padding-right: 5px;
}
&#10;#ccrjavgnrr .gt_left {
  text-align: left;
}
&#10;#ccrjavgnrr .gt_center {
  text-align: center;
}
&#10;#ccrjavgnrr .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}
&#10;#ccrjavgnrr .gt_font_normal {
  font-weight: normal;
}
&#10;#ccrjavgnrr .gt_font_bold {
  font-weight: bold;
}
&#10;#ccrjavgnrr .gt_font_italic {
  font-style: italic;
}
&#10;#ccrjavgnrr .gt_super {
  font-size: 65%;
}
&#10;#ccrjavgnrr .gt_footnote_marks {
  font-size: 75%;
  vertical-align: 0.4em;
  position: initial;
}
&#10;#ccrjavgnrr .gt_asterisk {
  font-size: 100%;
  vertical-align: 0;
}
&#10;#ccrjavgnrr .gt_indent_1 {
  text-indent: 5px;
}
&#10;#ccrjavgnrr .gt_indent_2 {
  text-indent: 10px;
}
&#10;#ccrjavgnrr .gt_indent_3 {
  text-indent: 15px;
}
&#10;#ccrjavgnrr .gt_indent_4 {
  text-indent: 20px;
}
&#10;#ccrjavgnrr .gt_indent_5 {
  text-indent: 25px;
}
&#10;#ccrjavgnrr .katex-display {
  display: inline-flex !important;
  margin-bottom: 0.75em !important;
}
&#10;#ccrjavgnrr div.Reactable > div.rt-table > div.rt-thead > div.rt-tr.rt-tr-group-header > div.rt-th-group:after {
  height: 0px !important;
}
&#10;tbody tr:last-child {
  border-bottom: 2px solid #ffffff00;
}
</style>
<table class="gt_table" data-quarto-disable-processing="false" data-quarto-bootstrap="false">
  <thead>
    <tr class="gt_heading">
      <td colspan="7" class="gt_heading gt_title gt_font_normal gt_bottom_border" style="font-family: Chivo; font-weight: 700;">Network Descriptive Stats</td>
    </tr>
    &#10;    <tr class="gt_col_headings">
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="Player name">Player name</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="OutDegrees">OutDegrees</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="InDegrees">InDegrees</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="Closeness">Closeness</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="Betweenness">Betweenness</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="PageRank">PageRank</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1" style="border-top-width: 0px; border-top-style: solid; border-top-color: black; font-family: Chivo; font-size: 14px; vertical-align: bottom; font-weight: 200; text-transform: uppercase;" scope="col" id="Eigenvector">Eigenvector</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td headers="Player name" class="gt_row gt_left">De Paul</td>
<td headers="OutDegrees" class="gt_row gt_right">537</td>
<td headers="InDegrees" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">509</td>
<td headers="Closeness" class="gt_row gt_right">0.354</td>
<td headers="Betweenness" class="gt_row gt_right">182</td>
<td headers="PageRank" class="gt_row gt_right">0.108</td>
<td headers="Eigenvector" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">1.000</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Molina</td>
<td headers="OutDegrees" class="gt_row gt_right">282</td>
<td headers="InDegrees" class="gt_row gt_right">284</td>
<td headers="Closeness" class="gt_row gt_right">0.324</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.060</td>
<td headers="Eigenvector" class="gt_row gt_right">0.708</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Romero</td>
<td headers="OutDegrees" class="gt_row gt_right">346</td>
<td headers="InDegrees" class="gt_row gt_right">285</td>
<td headers="Closeness" class="gt_row gt_right">0.346</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.057</td>
<td headers="Eigenvector" class="gt_row gt_right">0.719</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Otamendi</td>
<td headers="OutDegrees" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">547</td>
<td headers="InDegrees" class="gt_row gt_right">458</td>
<td headers="Closeness" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">0.364</td>
<td headers="Betweenness" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">275</td>
<td headers="PageRank" class="gt_row gt_right">0.089</td>
<td headers="Eigenvector" class="gt_row gt_right">0.861</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Enzo</td>
<td headers="OutDegrees" class="gt_row gt_right">451</td>
<td headers="InDegrees" class="gt_row gt_right">422</td>
<td headers="Closeness" class="gt_row gt_right">0.352</td>
<td headers="Betweenness" class="gt_row gt_right">69</td>
<td headers="PageRank" class="gt_row gt_right">0.090</td>
<td headers="Eigenvector" class="gt_row gt_right">0.837</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Acuña</td>
<td headers="OutDegrees" class="gt_row gt_right">173</td>
<td headers="InDegrees" class="gt_row gt_right">189</td>
<td headers="Closeness" class="gt_row gt_right">0.296</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.044</td>
<td headers="Eigenvector" class="gt_row gt_right">0.347</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Mac Allister</td>
<td headers="OutDegrees" class="gt_row gt_right">263</td>
<td headers="InDegrees" class="gt_row gt_right">292</td>
<td headers="Closeness" class="gt_row gt_right">0.304</td>
<td headers="Betweenness" class="gt_row gt_right">16</td>
<td headers="PageRank" class="gt_row gt_right">0.069</td>
<td headers="Eigenvector" class="gt_row gt_right">0.507</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Messi</td>
<td headers="OutDegrees" class="gt_row gt_right">345</td>
<td headers="InDegrees" class="gt_row gt_right">468</td>
<td headers="Closeness" class="gt_row gt_right">0.327</td>
<td headers="Betweenness" class="gt_row gt_right">181</td>
<td headers="PageRank" class="gt_row gt_right" style="background-color: #DB504A; color: #FFFFFF;">0.109</td>
<td headers="Eigenvector" class="gt_row gt_right">0.969</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Álvarez</td>
<td headers="OutDegrees" class="gt_row gt_right">112</td>
<td headers="InDegrees" class="gt_row gt_right">173</td>
<td headers="Closeness" class="gt_row gt_right">0.263</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.040</td>
<td headers="Eigenvector" class="gt_row gt_right">0.335</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Di María</td>
<td headers="OutDegrees" class="gt_row gt_right">145</td>
<td headers="InDegrees" class="gt_row gt_right">197</td>
<td headers="Closeness" class="gt_row gt_right">0.281</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.045</td>
<td headers="Eigenvector" class="gt_row gt_right">0.418</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Emiliano</td>
<td headers="OutDegrees" class="gt_row gt_right">162</td>
<td headers="InDegrees" class="gt_row gt_right">85</td>
<td headers="Closeness" class="gt_row gt_right">0.321</td>
<td headers="Betweenness" class="gt_row gt_right">43</td>
<td headers="PageRank" class="gt_row gt_right">0.020</td>
<td headers="Eigenvector" class="gt_row gt_right">0.194</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Tagliafico</td>
<td headers="OutDegrees" class="gt_row gt_right">143</td>
<td headers="InDegrees" class="gt_row gt_right">138</td>
<td headers="Closeness" class="gt_row gt_right">0.288</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.035</td>
<td headers="Eigenvector" class="gt_row gt_right">0.266</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Paredes</td>
<td headers="OutDegrees" class="gt_row gt_right">236</td>
<td headers="InDegrees" class="gt_row gt_right">198</td>
<td headers="Closeness" class="gt_row gt_right">0.317</td>
<td headers="Betweenness" class="gt_row gt_right">44</td>
<td headers="PageRank" class="gt_row gt_right">0.046</td>
<td headers="Eigenvector" class="gt_row gt_right">0.409</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Pezzella</td>
<td headers="OutDegrees" class="gt_row gt_right">49</td>
<td headers="InDegrees" class="gt_row gt_right">41</td>
<td headers="Closeness" class="gt_row gt_right">0.236</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.015</td>
<td headers="Eigenvector" class="gt_row gt_right">0.084</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Lautaro</td>
<td headers="OutDegrees" class="gt_row gt_right">60</td>
<td headers="InDegrees" class="gt_row gt_right">116</td>
<td headers="Closeness" class="gt_row gt_right">0.204</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.031</td>
<td headers="Eigenvector" class="gt_row gt_right">0.196</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Almada</td>
<td headers="OutDegrees" class="gt_row gt_right">12</td>
<td headers="InDegrees" class="gt_row gt_right">13</td>
<td headers="Closeness" class="gt_row gt_right">0.114</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.009</td>
<td headers="Eigenvector" class="gt_row gt_right">0.020</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Montiel</td>
<td headers="OutDegrees" class="gt_row gt_right">65</td>
<td headers="InDegrees" class="gt_row gt_right">76</td>
<td headers="Closeness" class="gt_row gt_right">0.229</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.020</td>
<td headers="Eigenvector" class="gt_row gt_right">0.164</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Martínez</td>
<td headers="OutDegrees" class="gt_row gt_right">149</td>
<td headers="InDegrees" class="gt_row gt_right">123</td>
<td headers="Closeness" class="gt_row gt_right">0.287</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.029</td>
<td headers="Eigenvector" class="gt_row gt_right">0.242</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Guido</td>
<td headers="OutDegrees" class="gt_row gt_right">60</td>
<td headers="InDegrees" class="gt_row gt_right">53</td>
<td headers="Closeness" class="gt_row gt_right">0.226</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.016</td>
<td headers="Eigenvector" class="gt_row gt_right">0.101</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Palacios</td>
<td headers="OutDegrees" class="gt_row gt_right">28</td>
<td headers="InDegrees" class="gt_row gt_right">28</td>
<td headers="Closeness" class="gt_row gt_right">0.214</td>
<td headers="Betweenness" class="gt_row gt_right">85</td>
<td headers="PageRank" class="gt_row gt_right">0.022</td>
<td headers="Eigenvector" class="gt_row gt_right">0.037</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Gómez</td>
<td headers="OutDegrees" class="gt_row gt_right">57</td>
<td headers="InDegrees" class="gt_row gt_right">67</td>
<td headers="Closeness" class="gt_row gt_right">0.210</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.020</td>
<td headers="Eigenvector" class="gt_row gt_right">0.138</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Dybala</td>
<td headers="OutDegrees" class="gt_row gt_right">12</td>
<td headers="InDegrees" class="gt_row gt_right">18</td>
<td headers="Closeness" class="gt_row gt_right">0.088</td>
<td headers="Betweenness" class="gt_row gt_right">22</td>
<td headers="PageRank" class="gt_row gt_right">0.010</td>
<td headers="Eigenvector" class="gt_row gt_right">0.026</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Foyth</td>
<td headers="OutDegrees" class="gt_row gt_right">3</td>
<td headers="InDegrees" class="gt_row gt_right">3</td>
<td headers="Closeness" class="gt_row gt_right">0.065</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.008</td>
<td headers="Eigenvector" class="gt_row gt_right">0.000</td></tr>
    <tr><td headers="Player name" class="gt_row gt_left">Correa</td>
<td headers="OutDegrees" class="gt_row gt_right">4</td>
<td headers="InDegrees" class="gt_row gt_right">5</td>
<td headers="Closeness" class="gt_row gt_right">0.064</td>
<td headers="Betweenness" class="gt_row gt_right">0</td>
<td headers="PageRank" class="gt_row gt_right">0.008</td>
<td headers="Eigenvector" class="gt_row gt_right">0.004</td></tr>
  </tbody>
  &#10;  <tfoot class="gt_footnotes">
    <tr>
      <td class="gt_footnote" colspan="7"> <span style = "color:##254441;"> Highest values </span></td>
    </tr>
  </tfoot>
</table>
</div>

The summary shows first how Argentina played. This is a team that favored patient buildup up from the back, this helps explains Otamendi’s high betweenness and out-degree scores. It also depended a lot on advancing the ball through central spaces, this is reflected by the fact that the players with the highest between scores are midfielders and, of course, Lionel Messi and they had few if any true out and out wingers capable of hugging the touchline and producing width in the wide spaces. When checking the important players firstly with the page rank algorithm, we see that Messi ranks highest, but RDP ranks highest when using the eigenvector centrality. However, this shows how the algorithms evaluate the importance of elements in a network. Despite the difference, Messi is second in the EigENVECTOR WHILE RDP IS SECOND USING Page Rank; again, strengthening the team’s right side was where the magic happened.

In conclusion, we see just how important Rdp was to Argentin’s Worlcup Triumph.
