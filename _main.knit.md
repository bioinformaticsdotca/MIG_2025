--- 
title: "Microbial Genomics 2025"
author: "Faculty: Jared Simpson, Gary van Domselaar, Andrew McArthur, Rob Beiko, Fiona Brinkman"
date: "November 20-22, 2025"
site: bookdown::bookdown_site
documentclass: book
bibliography: [book.bib, packages.bib]
url: https://bioinformaticsdotca.github.io/MIG-2511/ 
cover-image: img/bioinformatics_logo.png
description: |
  Workshop website for the 2025 Microbial Genomics Canadian Bioinformatics Workshop
link-citations: yes
github-repo: bioinformaticsdotca/MIG-2511
favicon: img/favicon.ico
---

# (PART) Introduction {-}

# Workshop Info

Welcome to the 2025 Microbial Genomics Canadian Bioinformatics Workshop webpage!  

## Pre-work

<!--[You can find your pre-work here.](LINK TO PREWORK)-->

## Class Photo

Coming soon! 

## Schedule


```{=html}
<style>
    :root {
      --schedule-primary-color: #4A6BFF;
      --schedule-border-color: #EAECEF;
      --schedule-text-color: #555;
    }
    .schedule-card {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      border: 1px solid var(--schedule-border-color);
      border-radius: 12px;
      margin: 2em 0;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      overflow: hidden;
    }
    .schedule-tabs {
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid var(--schedule-border-color);
      background-color: #fff;
    }
    .schedule-tabs-wrapper {
      position: relative;
      flex-grow: 1;
      overflow: hidden;
    }
    .schedule-tabs-wrapper::before,
    .schedule-tabs-wrapper::after {
      content: '';
      position: absolute;
      top: 0;
      bottom: 0;
      width: 50px;
      pointer-events: none;
      transition: opacity 0.2s;
      opacity: 0;
    }
    .schedule-tabs-wrapper::before {
      left: 0;
      background: linear-gradient(to left, rgba(255,255,255,0), #fff 70%);
    }
    .schedule-tabs-wrapper::after {
      right: 0;
      background: linear-gradient(to right, rgba(255,255,255,0), #fff 70%);
    }
    .schedule-tabs-wrapper.scrolled-left::before { opacity: 1; }
    .schedule-tabs-wrapper.scrolled-right::after { opacity: 1; }
    
    .schedule-tab-buttons {
      display: flex;
      overflow-x: auto;
      white-space: nowrap;
      -ms-overflow-style: none;
      scrollbar-width: none;
      scroll-behavior: smooth;
    }
    .schedule-tab-buttons::-webkit-scrollbar { display: none; }
    
    .timezone-selector-container {
      display: flex;
      align-items: center;
      gap: 0.75em;
      padding: 0 20px;
    }
    .timezone-selector-container label {
      font-size: 0.9em;
      color: var(--schedule-text-color);
      font-weight: 500;
    }
    .schedule-tabs select {
      padding: 6px 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
      background-color: #fff;
    }
    .schedule-tab {
      padding: 14px 20px;
      cursor: pointer;
      border-bottom: 3px solid transparent;
      margin-bottom: -1px;
      color: var(--schedule-text-color);
      font-weight: 500;
    }
    .schedule-tab.active {
      color: var(--schedule-primary-color);
      border-bottom-color: var(--schedule-primary-color);
    }
    .schedule-panel { display: none; }
    .schedule-panel.active { display: block; }
    .schedule-table { width: 100%; border-collapse: collapse; }
    .schedule-table th, .schedule-table td {
      text-align: left;
      padding: 14px 20px;
      border-bottom: 1px solid var(--schedule-border-color);
    }
    .schedule-table th {
      color: #888;
      font-size: 0.8em;
      font-weight: 600;
      text-transform: uppercase;
      background-color: #F8F9FA;
    }
    .schedule-table tr:last-child td { border-bottom: none; }
    
    /* --- RULE FOR BREAKS AND PAUSES --- */
    .schedule-table tr.is-break td {
      font-style: italic;
      font-size: 0.95em;
      color: #777;
    }
    
    /* --- NEW: RULE FOR 'OTHER' TYPE (More Visible) --- */
    .schedule-table tr.is-other td {
      background-color: #f0f4ff; /* A light blue background */
      font-weight: 500; /* Slightly bolder text */
    }
    .schedule-table tr.is-other td:first-child {
      border-left: 4px solid var(--schedule-primary-color);
    }
  </style>
<div class="schedule-card">
<div class="schedule-tabs" id="schedule-tabs-container"></div>
<div class="schedule-content" id="schedule-panels-container"></div>
</div>
<script>
    document.addEventListener("DOMContentLoaded", function() {
      const scheduleData = [{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Zoom Opens,activity,09:45,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,\"Welcome (Regional Coordinator)\",activity,10:00,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Compute Setup: AWS Review (Zhibin Lu),activity,10:30,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Module 1 Lecture: Genome Assembly (Instructor: Jared Simpson),activity,11:00,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Break (30min),break,12:00,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Module 2 Lecture: Genome Annotation (Gary van Domselaar),activity,12:30,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Lunch (1 hr),break,13:30,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Module 2 Lab: Genome Annotation (Gary van Domselaar),activity,14:30,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,Break (30min),break,15:30,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,(contd) Module 2 Lab: Genome Annotation (Gary van Domselaar),activity,16:00,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"},{"day_label,date,activity,type,time_1,timezone_1_label":"November 20,2025-11-20,\"Finished Optional: Integrative Assignment (TA)\",break,17:00,\"Time (ET)\"","...2":"NA","...3":"NA","...4":"NA","...5":"NA","...6":"NA","...7":"NA"}];
      const tabsContainer = document.getElementById("schedule-tabs-container");
      const panelsContainer = document.getElementById("schedule-panels-container");

      if (scheduleData.length === 0) return;

      const timezones = [];
      const firstRow = scheduleData[0];
      for (const key in firstRow) {
        if (key.match(/timezone_\d+_label/)) {
          const index = key.match(/\d+/)[0];
          timezones.push({ index: index, label: firstRow[key] });
        }
      }
      const days = [...new Set(scheduleData.map(row => row.day_label))];
      
      const tabsWrapper = document.createElement("div");
      tabsWrapper.className = "schedule-tabs-wrapper";
      const tabButtonsContainer = document.createElement("div");
      tabButtonsContainer.className = "schedule-tab-buttons";
      tabsWrapper.appendChild(tabButtonsContainer);
      tabsContainer.appendChild(tabsWrapper);

      days.forEach((day, dayIndex) => {
        const tab = document.createElement("div");
        tab.className = "schedule-tab";
        tab.dataset.target = `panel-${dayIndex}`;
        tab.textContent = day;
        tabButtonsContainer.appendChild(tab);
      });

      if (timezones.length > 1) {
        const selectorContainer = document.createElement("div");
        selectorContainer.className = "timezone-selector-container";
        let selectorHtml = `<label for="tz-selector">Timezone</label>
                            <select id="tz-selector">`;
        timezones.forEach(tz => {
          selectorHtml += `<option value="${tz.index}">${tz.label}</option>`;
        });
        selectorHtml += `</select>`;
        selectorContainer.innerHTML = selectorHtml;
        tabsContainer.appendChild(selectorContainer);
      }
      
      const tzSelector = document.getElementById("tz-selector");

      days.forEach((day, dayIndex) => {
        panelsContainer.innerHTML += `<div class="schedule-panel" id="panel-${dayIndex}"></div>`;
      });
      
      const tabs = document.querySelectorAll(".schedule-tab");
      const panels = document.querySelectorAll(".schedule-panel");

      function renderTables() {
        const selectedTzIndex = tzSelector ? tzSelector.value : timezones[0].index;
        const timeCol = `time_${selectedTzIndex}`;
        let selectedTzLabel = tzSelector ? tzSelector.options[tzSelector.selectedIndex].text : timezones[0].label;
        
        panels.forEach((panel, dayIndex) => {
          const day = days[dayIndex];
          const dayEvents = scheduleData.filter(row => row.day_label === day);
          let tableHtml = `<table class="schedule-table"><thead><tr>
                               <th style="width:25%;">${selectedTzLabel}</th>
                               <th>Activity</th>
                               </tr></thead><tbody>`;
          dayEvents.forEach(row => {
            const type = row.type ? row.type.toLowerCase() : "";
            let rowClass = "";

            if (type === "break" || type === "pause") {
              rowClass = "class='is-break'";
            } else if (type === "other") {
              rowClass = "class='is-other'";
            }
            
            tableHtml += `<tr ${rowClass}><td>${row[timeCol] || ""}</td><td>${row.activity || ""}</td></tr>`;
          });
          tableHtml += `</tbody></table>`;
          panel.innerHTML = tableHtml;
        });
      }

      function switchTab(targetId) {
        tabs.forEach(tab => tab.classList.remove("active"));
        panels.forEach(panel => panel.classList.remove("active"));
        
        const activeTab = document.querySelector(`[data-target='${targetId}']`);
        const activePanel = document.getElementById(targetId);
        
        if (activeTab) {
          activeTab.classList.add("active");
          activeTab.scrollIntoView({ behavior: "smooth", block: "nearest", inline: "center" });
        }
        if (activePanel) {
          activePanel.classList.add("active");
        }
      }
      
      function updateScrollIndicators() {
        const el = tabButtonsContainer;
        const scrollLeft = Math.round(el.scrollLeft);
        const scrollWidth = Math.round(el.scrollWidth);
        const clientWidth = Math.round(el.clientWidth);
        
        const hasOverflow = scrollWidth > clientWidth;
        tabsWrapper.classList.toggle("scrolled-left", hasOverflow && scrollLeft > 0);
        const isAtEnd = scrollLeft >= scrollWidth - clientWidth;
        tabsWrapper.classList.toggle("scrolled-right", hasOverflow && !isAtEnd);
      }

      tabButtonsContainer.addEventListener("click", e => {
        if (e.target.classList.contains("schedule-tab")) {
          switchTab(e.target.dataset.target);
        }
      });

      if (tzSelector) {
        tzSelector.addEventListener("change", renderTables);
      }
      
      tabButtonsContainer.addEventListener("scroll", updateScrollIndicators, { passive: true });
      window.addEventListener("resize", updateScrollIndicators);

      renderTables();

      // --- LOGIC TO ACTIVATE CURRENT DAY ---
      let initialTabIndex = 0;

      const today = new Date();
      const monthNames = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
      const monthName = monthNames[today.getMonth()];
      const day = today.getDate();
      const year = today.getFullYear();
      const todayString = `${monthName} ${day}, ${year}`;

      const todayEvent = scheduleData.find(row => row.date === todayString);

      if (todayEvent) {
        const dayIndex = days.findIndex(day => day === todayEvent.day_label);
        if (dayIndex !== -1) {
          initialTabIndex = dayIndex;
        }
      }

      if (tabs.length > initialTabIndex) {
        const initialTabId = `panel-${initialTabIndex}`;
        switchTab(initialTabId);
      }
      // --- END OF CURRENT DAY LOGIC ---

      setTimeout(updateScrollIndicators, 100);
    });
  </script>
```

<!--chapter:end:index.Rmd-->

# Meet Your Faculty

<!--#### NAME

<img src="./img/faculty/MISSINGHEADSHOT.PNG" width="200" alt="Photo of NAME">

>JOB TITLE <br>
INSTITUTION <br>
LOCATION
>
> --- CONTACT INFO, IF PROVIDED

BIO GOES HERE-->


<!--chapter:end:001-faculty.Rmd-->

<!--
IF YOUR WORKSHOP DOES NOT INCLUDE COMPUTE:
- REMOVE "AND COMPUTE SETUP" FROM THE TOP-LEVEL HEADER
- DELETE THE LAST SECTION (COMPUTE SETUP)

IF YOUR WORKSHOP INCLUDES COMPUTE:
- AFTER THE WORKSHOP, ADD DATA DOWNLOAD LINKS, AWS MACHINE IMAGE INSTRUCTIONS, ETC.
- IF IT IS MORE APPROPRIATE, YOU CAN INCLUDE THE DATA DOWNLOAD LINKS IN EACH OF THE MODULES.
-->

# Data and Compute Setup

#### Course data downloads
Coming soon!

#### Compute setup
Coming soon!



<!--chapter:end:002-computing.Rmd-->

# (PART) Modules {-}

# Module 1 Genome Assembly

## Lecture

<!--<iframe width="640" height="360" src="YOUTUBE EMBED LINK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
-->

<!--<iframe src="GOOGLE SLIDES LINK/preview" width="640" height="480" allow="autoplay"></iframe>  
-->

## Lab

<!--chapter:end:010-module-1.Rmd-->

# Module 2 Genome Annotation

## Lecture


## Lab

<!--chapter:end:020-module-2.Rmd-->

# Module 3 Antimicrobial Resistant Gene (AMR) Analysis

## Lecture


## Lab

<!--chapter:end:030-module-3.Rmd-->

# Module 4 Mobile Genetic Elements

## Lecture


## Lab

<!--chapter:end:040-module-4.Rmd-->

