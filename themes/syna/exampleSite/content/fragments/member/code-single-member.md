+++
fragment = "content"
weight = 111
+++

<details><summary>Code (index)</summary>

```
+++
fragment = "member"
#disabled = false
date = "2021-09-01"
weight = 110
background = "secondary"

title = "Single Member Fragment"
#subtitle = "Highly motivated Gophers"
#title_align = "left" # Default is center, can be left, right or center
+++
```
</details>

<details>
<summary>Code (subitem)</summary>

```
+++
title = "Huge Gopher"
weight = 0
date = "2021-09-01"
#disabled = true

position = "Lead Gopherineer"
company = "Okkur Labs"

reports_to = "CTO"
lives_in = "[Munich, Germany](https://www.google.com/maps/place/Munich,+Germany/)"
scope = [
  "UX for [Food Dashboard](#)",
  "Maintainer for [Goper Team A](#)",
  "Gopher [Community Administration](#)"
]

[[icons]]
  icon = "fab fa-linkedin-in"
  text = "Linkedin"
  url = "#"

[asset]
  image = "hugegopher.png"
+++

Hugely huge Gopher

Some more text to showcase the capabilities:
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Curabitur a lorem urna.
Quisque in neque malesuada, sollicitudin nunc porttitor, ornare est.
Praesent ante enim, bibendum sed hendrerit et, iaculis laoreet felis.
Morbi efficitur dui sit amet orci porttitor, nec tincidunt turpis elementum.
```
</details>
