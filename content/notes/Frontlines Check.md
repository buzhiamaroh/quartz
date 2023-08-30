---
title: "Frontlines Check"
katex: true
tags:
- PVP
toc: false
---
## What Frontlines map is it today?
{{< rawhtml >}}
<p id="frontlines">

</p>
<script>
let div = document.getElementById("frontlines");
let today = new Date();
let start = new Date("08/29/2023");
let roulette = ["Seal Rock", "Shatter", "Onsaal Hakar"];
console.log(start.getTime());
let dayIndex = Math.floor((today.getTime() - start.getTime()) / (1000 * 60 * 60 * 24)) % 3;
console.log(dayIndex);
div.innerHTML = roulette[dayIndex];
</script>
{{< /rawhtml >}}