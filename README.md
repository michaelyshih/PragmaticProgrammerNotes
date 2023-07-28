# PragmaticProgrammerNotes

This is my summary of The Pragmatic Programmer, by Andrew Hunt and David Thomas. I use it while learning and as a quick reference. It is not intended to be a standalone substitution of the book so if you really want to learn the concepts here presented, buy and read the book and use this repo as a ref and guide.

If you are the publisher and think this repo should not be public, just write me an email at ... and I will make it private.

<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->
# Table of Contents
- [Preface](#preface)
- [Table of Contents](#table-of-contents)
- [Chapter 1. A Pragmatic Philosophy](#chapter-1-a-pragmatic-philosophy)
	- [1.-The Cat Ate My Source Code](#1-the-cat-ate-my-source-code)
	- [2.-Software Entropy](#2-software-entropy)
	- [3.-Stone Soup and Boiled Frogs](#3-stone-soup-and-boiled-frogs)
	- [4.-Good enough soup](#4-good-enough-soup)
	- [5.-Your Knowledge Portfolio](#5-your-knowledge-portfolio)
	- [6.-Communicate](#6-communicate)
- [Chapter 2. A Pragmatic Approach](#chapter-2-a-pragmatic-approach)
	- [7.-The Evils of Duplication](#7-the-evils-of-duplication)
	- [8.-Orthogonality](#8-orthogonality)
	- [9.-Reversibility](#9-reversibility)
	- [10-Tracer Bullets](#10-tracer-bullets)
	- [11.-Prototypes and Post-it Notes](#11-prototypes-and-post-it-notes)
	- [12.-Domain Languages](#12-domain-languages)
	- [13.-Estimating](#13-estimating)
- [Chapter 3. The Basic Tools](#chapter-3-the-basic-tools)
	- [14.-The Power of Plain Text](#14-the-power-of-plain-text)
	- [15.-Shell Games](#15-shell-games)
	- [16.-Power Editing](#16-power-editing)
	- [17.-Source Code Control](#17-source-code-control)
	- [18.-Debugging](#18-debugging)
	- [19.-Text Manipulation](#19-text-manipulation)
	- [20.-Code Generators](#20-code-generators)
- [Chapter 4. A Pragmatic Paranoia](#chapter-4-a-pragmatic-paranoia)
	- [21.-Design by Contract](#21-design-by-contract)
	- [22.-Dead Programs Tell No Lies](#22-dead-programs-tell-no-lies)
	- [23.-Assertive Programming](#23-assertive-programming)
	- [24.-When to Use Exceptions](#24-when-to-use-exceptions)
	- [25.-How to Balance Resources](#25-how-to-balance-resources)
- [Chapter 5. Bend or Break](#chapter-5-bend-or-break)
	- [26.-Decoupling and the Law of Demeter](#26-decoupling-and-the-law-of-demeter)
	- [27.-Metaprogramming](#27-metaprogramming)
	- [28.- Temporal Coupling](#28-temporal-coupling)
	- [29.-It's Just a View](#29-its-just-a-view)
	- [30.-Blackboards](#30-blackboards)
- [Chapter 6. While you are coding](#chapter-6-while-you-are-coding)
	- [31.-Program by Coincidence](#31-program-by-coincidence)
	- [32.-Algorithm Speed](#32-algorithm-speed)
	- [33.-Refactoring](#33-refactoring)
	- [34.-Code That's Easy to Test](#34-code-thats-easy-to-test)
	- [35.-Evil Wizards](#35-evil-wizards)
- [Chapter 7. Before the project](#chapter-7-before-the-project)
	- [36.-The Requirements Pit](#36-the-requirements-pit)
	- [37.-Solving Impossible Puzzles](#37-solving-impossible-puzzles)
	- [38.-Not Until You're Ready](#38-not-until-youre-ready)
	- [39.-The Specification Trap](#39-the-specification-trap)
	- [40.-Circles and Arrows](#40-circles-and-arrows)
- [Chapter 8. Pragmatic Projects](#chapter-8-pragmatic-projects)
	- [41.-Pragmatic Teams](#41-pragmatic-teams)
	- [42.-Ubiquitous Automation](#42-ubiquitous-automation)
	- [43.-Ruthless testing](#43-ruthless-testing)
	- [44.-It's All Writing](#44-its-all-writing)
	- [45.- Great Expectations](#45-great-expectations)
- [Quick Reference](#quick-reference)
	- [Tips](#tips)
	- [CheckList](#checklist)
		- [Languages To Learn](#languages-to-learn)
		- [The WISDOM Acrostic](#the-wisdom-acrostic)
		- [How to Maintain Orthogonality](#how-to-maintain-orthogonality)
		- [Things to prototype](#things-to-prototype)
		- [Architectural Questions](#architectural-questions)
		- [Debugging Checklist](#debugging-checklist)
		- [Law of Demeter for Functions](#law-of-demeter-for-functions)
		- [How to Program Deliberately](#how-to-program-deliberately)
		- [When to Refactor](#when-to-refactor)
		- [Cutting the Gordian Knot](#cutting-the-gordian-knot)
		- [Aspects of Testing](#aspects-of-testing)
<!-- /TOC -->

# Preface
**quotes 1: This isn't a one-time audit of current practices

### Notes
- Great lawns need small amounts of daily care, and so do great programmers. Every day, work to refine the skills you have and to add new tools to your repertoire. Unlike the Eton lawsns, you'll start seeing results in a matter of days.

-Appendix A contains a set of reources: periodicals, books, and pro org.

-Appendix B contains exervises

**modularity applies to code, designs, documentation, and team organization.

# Chapter 1. A Pragmatic Philosohpy

### Notes
- Think beyond the immediate problem, trying to place it in its larger context, always trying to be aware of the bigger picture.

- Being responsible, Prgamtic Programmers won't sit  idly by and watch their projects fall apart through neglect.

### Tip 1: Care About Your Craft**

Why spend your life developing software unless you care about doing it well?

### Tip 2: Think! About Your Work**

Turn off the autopilot and take control. Constantly critique and appraise your work.

## 1.-The Cat Ate My Source Code

### Tip 3: Provide Options, Don't Make Lame Excuses**

### Notes
- Despite throrough testing, good documentation, and solid automation,things go wrong. Deliveries are late. Unforseen tech prob arise.

- Instead of excuses, provide options. Don't say it can't be done; explain what can be done to salvage the situation.

**quotes 2: It is up to you to to provide solutions, not excuses.

- If there was a reisk that the vendor wouldn't come through for you, then you should have had a contingecy plan. If the disk crashes-- taking all your code with it-- and you don't haave a backup. it's Your fault.

- Before telling boss why something can't be done, is late, or broken. Ask rubber ducky if reasonable. How it'll sound to boss.

- "Have you tried... / Did you consider..." - you already know what they're going to say so save them the trouble

- "Prototypign and post-it notes / better testing? / additional resources?

- How do you react when someone, such as a bank teller, an auto mehcanic, or a cleark-- comes to you with a lame excuse? What do you think of them and their company as aresult?

## 2.-Software Entropy
