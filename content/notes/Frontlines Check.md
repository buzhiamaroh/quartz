---
title: "Frontlines Check"
katex: true
tags:
- PVP
toc: false
---
## What Frontlines map is it today?{.center}
{{< rawhtml >}}
<p id="frontlines" class="center">

</p>
<script>
let div = document.getElementById("frontlines");
let today = new Date();
let start = new Date("08/29/2023 10:00");
let roulette = ["Seal Rock", "Shatter", "Onsaal Hakar"];
let dayIndex = Math.floor((today.getTime() - start.getTime()) / (1000 * 60 * 60 * 24)) % 3;
div.innerHTML = `<strong style="font-size: 18px">Today:</strong> ${roulette[dayIndex]} <br> <strong style="font-size: 18px">Tomorrow:</strong> ${roulette[(dayIndex+1)%3]}`;
</script>
{{< /rawhtml >}}