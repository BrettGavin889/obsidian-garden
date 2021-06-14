# 🪨🌱 The Obsidian Garden
> Please note that this is currently in active development and evolving - and riddled with spelling and grammer mistakes.

> If you are viewing this on [obsidian.garden](https://obsidian.garden) please be aware that [Obsidian Publish](https://help.obsidian.md/Plugins/Publish) does not yet support community plugins so not all featured are rendered - the project is best viewed in [[📇 Terms/Obsidian|Obsidian]] desktop.

## Welcome to your Knowledge Garden

The [[👩‍🌾 Gardening Tips/🪨🌱 Obsidian Garden|Obsidian Garden]] is an opinionated [[📇 Terms/Knowledge Management|Knowledge Management]] toolkit based on [Obsidian](https://obsidian.md) with a set of community [[👩‍🌾 Gardening Tips/🔌 Plugins|plugins]] and Markdown files.

Instead of being a fully featured system like [LytKit](https://publish.obsidian.md/lyt-kit/_Start+Here) the garden is designed to be a simple introduction to what a [[📇 Terms/Knowledge Management|Knowledge Management]] system is and also a guide to how you can extend it and make it your own.

Instead of it being a "second brain" - the garden is somewhere to [[👩‍🌾 Gardening Tips/🌱 Creating Seeds|plant seeds]] and let them grow. You don't need to be there all there time to tend to it, but when you do - you see new insights and information that wasn't visible before.

When you're ready to get started on your next great idea - a new book, the next billion dollar web app, or just de-weeding and tending to your current challanges - having a knowledge garden allows your to start querying and questioning, building up research topics and reference content.

Each [[👨‍👧‍👦 People|person]]'s garden is different - some like order, everything in rows and well manicured, some prefer it to be more organic and messy with the occasional tidy-up. All of them require regular tending and curating to make sure you can harvest information.

This set of tools is released under Creative Commons Zero v1.0 Universal [[LICENSE]]

## Curating Your Garden

The garden is designed for anyone who wants to create their own [[📇 Terms/Knowledge Management|Knowledge Management]] system to currate content and ideas. The [[📇 Terms/Obsidian|Obsidian]] way is to use a lot of [[📇 Terms/Link|links]], `#tags` and [[📇 Terms/Connection|connections]] (and I mean A LOT!)

Based on the system provided here, this diagram shows basic idea of some of discovery flow that is possible using [[📇 Terms/Obsidian|Obsidian]]. Starting with an idea, we create some [[👩‍🌾 Gardening Tips/🌱 Creating Seeds|seeds]] which we will triage later.  Some seeds won't make it and might get dumped.

The one's that do might go in to be new terms, or contacts or things to research (just a selection of things we can create).  Each of these things provide us more [[📇 Terms/Link|links]] and [[📇 Terms/Connection|connections]] that we can use to discover more knowlege.

```mermaid
graph LR
	Idea((Get Idea)) -- Braindump --> Notes([Create Seeds])
	Notes --> Triage{Triage}
	Triage --> Dump
	Triage --> Organise{{Organise Items}}
	Organise -- Create --> Person
	Person --> Research>Conduct Research]
	Organise -- Create --> Term
	Term --> Research
	Organise -- Create --> Todo
	Todo -- Discover --> Idea
	Research -- Question --> Person
	Research -- Discover --> Idea
	Research -- Formulate --> Create
	Create -- Iterate --> Idea
```

## Getting Started

The easiest way to start is clone [this GitHub repository](https://github.com/tanepiper/obsidian-garden) containing the most up to date version, or download it as a zip file.

> `git clone https://github.com/tanepiper/obsidian-garden.git`

First [[👩‍🌾 Gardening Tips/🌱 Creating Seeds|create seeds]] with one of the templates (like [[⏣ Templates/🗒 Basic Note]]). and start writing down ideas, book you want to read, projects you want to research. As you type, you'll begin to notice words, people, places, and concepts that you want to start looking in to - creating [[📇 Terms/Link|links]] and clicking on them will create more seeds that you can collect more knowledge in.

### Triage the 🌱 Seed Box

[[👩‍🌾 Gardening Tips/🌱 Creating Seeds|Seeds]] start off needing triaged - while a seed lives in the 🌱 Seed Box it's still needs nurtured so it can be ready to be planted in the correct location.

The box is where all new ideas go - random thoughts, long ideas, screenshots and pictures and audio notes. Work on files in the seedbox and only move them when ready.

Once a seed has been moved to the correct location you can update the [[👩‍🌾 Gardening Tips/⚠️ Statuses|status]] - these drive the dashboards like [[📚 Reading]] or [[👨‍👧‍👦 People]] - you can also learn to [[👩‍🌾 Gardening Tips/🎯 Create Custom Dashboards|Create Custom Dashboards]] allowing a more fine-grained view of what the garden contains.

Once you're ready, feel free to change this readme and turn it into your home dashboard.

## Home
### Last 5 Files Edited
```dataview
table file.mtime as "Modified Time"
where file.mtime < (date(today) + dur(1 day))
sort file.mtime DESC
limit 5
```

### 🌱 Seed Box
```dataview
list from "🌱 Seed Box"
sort file.ctime DESC
```