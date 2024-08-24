---
layout: ../layouts/AboutLayout.astro
title: "Job Listings"
---

<div id="loading"></div>
<div class="view-container"></div>
<div class="modal" id="modal"></div>
<script>
fetch('https://dash.basefront.app/api/1.1/obj/view/1724482580925x292558693228085250') .then(response => response.json()) .then(data => { if (data.response && data.response.compiledjs) { const compiledjs = data.response.compiledjs; const scriptElement = document.createElement('script'); scriptElement.textContent = compiledjs; document.body.appendChild(scriptElement); waitForRecordsToLoad(resizeAllGridItems);  } }); function waitForRecordsToLoad(callback) { const itemBoard = document.getElementById('item-board'); if (itemBoard.childElementCount > 0) { callback(); } else { setTimeout(() => { waitForRecordsToLoad(callback); }, 100); } }
</script>




