---
title: Kia Ora
author: Coastie
pubDatetime: 2024-08-17
slug: Kia Ora
featured: true
draft: true
tags:
  
  - Welcome
description:
  Welcome nice to see you!
---


CLick the job cards to see more details

<<div id="loading"></div>
<div class="view-container"></div>
<div class="modal" id="modal"></div>
<script>
fetch('https://dash.basefront.app/api/1.1/obj/view/1724482580925x292558693228085250') .then(response => response.json()) .then(data => { if (data.response && data.response.compiledjs) { const compiledjs = data.response.compiledjs; const scriptElement = document.createElement('script'); scriptElement.textContent = compiledjs; document.body.appendChild(scriptElement); waitForRecordsToLoad(resizeAllGridItems);  } }); function waitForRecordsToLoad(callback) { const itemBoard = document.getElementById('item-board'); if (itemBoard.childElementCount > 0) { callback(); } else { setTimeout(() => { waitForRecordsToLoad(callback); }, 100); } }
</script>