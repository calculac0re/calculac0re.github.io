---
title: "HTB CDSA: From Zero to Hero"
date: 2024-07-26T22:40:27-07:00
draft: false
showToc: true
TocOpen: false
hidemeta: false
comments: false
description: A comprehensive breakdown of Hack The Box's blue team certification
canonicalURL: "https://calculac0re.net/posts/htb-cdsa-from-zero-to-hero/"
disableHLJS: false
disableShare: true
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: true
ShowRssButtonInSectionTermList: false
UseHugoToc: true
---

## Introduction

HTB Certified Defensive Security Analyst (CDSA) is a new highly hands-on blue team certification by Hack The Box. It was launched on HTB Academy in September of 2023 and has slowly been gaining holders, up to 132 at the time of this post. The entry-to-intermediate-level certification is curated to industry newcomers and professionals alike and teaches students SOC operations, including event log analysis, SIEM fundamentals, threat hunting, and incident reporting.

I started the course in February 2024 and finished in March, and took the exam four days later. I received my results the following month.

For some background, I am a college student that has been studying cybersecurity for 4 years, and I have no work experience in the field.

## The Cost

On the HTB Academy website, they state that you can get this certification for $490. In reality, The $490 gives you access to more content than just the CDSA course, and it is well worth if you plan on doing more than the one course or certification. If you only are looking to get CDSA, then you can get the certification for only $316 (one month of Platinum sub + one month of Gold sub + exam voucher).

If you are a student, you can get the Student sub which only costs $8 a month, and you can potentially get the certification for only $226. Not only do you get access to the CDSA course which contains 15 modules, but you also get access to an additional 30+ modules that cover the Certified Bug Bounty Hunter (CBBH) and Certified Penetration Testing Specialist (CPTS) certifications. It's the best value you can get, and I strongly encourage you to get it if you are a student.

## The Course

The content of the CDSA course is provided via learning modules, where each module focuses on a particular subject. Some of the subjects include `Incident Handling Process`, `Introduction to Threat Hunting & Hunting with Elastic`, and `Detecting Windows Attacks with Splunk`. The course also touches on advanced topics, such as `Introduction to Malware Analysis` and `Introduction to Digital Forensics`. These modules, while introductory, are meant to arm students with the necessary skills needed to occasionally perform more advanced SOC operations when needed.

Each module is split into different sections, with each section covering different aspects of the topic of the module. They start with an introduction to the topic, and each section afterward covers the nitty-gritty, going in-depth on each aspect. The content is provided via text; no videos are provided. Sections may also provide a target VM for you to spawn and interact with. The targets are hosted entirely on HTB Academy, so students are not expected to run them on their own computers. Some sections will have questions that need to be answered in order to complete the module. These questions are based on the current and, usually, prior sections, and the questions range from simple terminology to finding flags or certain information within the target VM. The exercises progressively become more challenging as you go through the module, demanding a healthy understanding of the content. Simply copying and pasting commands will not be sufficient.

At the end of each module is a skills assessment where you are tested on your understanding of everything that was taught. You are given a target VM with which you interact with and answer questions based on the given scenario. You can expect everything you learned in the module to be utilized within the skills assessment, and you are often required to think outside the box to find the answers to each question.

For the exercises, you can either use your own VM or you can use the Pwnbox, an in-browser VM provided by HTB Academy, to interact with the targets.

I found the course to be extremely well-put together and easy to follow. It spans 15 modules, and it is laid out to start with the fundamentals and gradually progress to more intermediate topics, a "zero to hero" approach. Out of all the exercises in the course, there was only one question that I felt was a bit unfair, but other than that, they were excellently put together. The lab environments were also pretty stable, albeit a bit slow due to the nature of RDP. There were moments where I would lose connection to the targets, but most of these issues were attributed to a problem on my end.

## The Exam

The exam involves two security incidents that you are tasked investigate and report on. You are given 7 days to submit 17 out of 20 flags for the first incident and submit a report for both incidents. The report should adhere strictly to the layout described in the `Security Incident Reporting` module, barring some sections relying on operations that can't be emulated within a lab environment such as eradication and recovery. You are expected to provide an in-depth technical analysis of the incident, supplying ample evidence and analysis to prove that an incident has taken place.

The provided lab environment was very stable, more stable than the module exercises even. I did not have to reach out to support for any maintenance. You can either use your own VM or the Pwnbox to complete the exam. I would like to talk more about the lab environment, but I don't want to spoil anything that could be sensitive.

For the report, I used Sysreptor, which has [HTB exam report templates](https://docs.sysreptor.com/htb-reporting-with-sysreptor/) that you are encouraged to use (with the possible exception of the CWEE report; the deliverable for this exam is different). The template helped save a ton of time as I didn't have to spend any time formatting the report. It's also utilizes Markdown, making the report very easy to write.

I took the exam during a full college workload, which kind of sucked because I was only able to finish the course after spring break. I found 17 flags on the first day of the exam and found all 20 on the next day. I spent the day after investigating the second incident. The last 4 days I spent writing the report, which I am glad that I did because I tend to be slow when writing reports. I received my results about a month after submitting the report.

I found the lab to be quite fun and engaging. It felt "realistic," at least according to my understanding of incident response. It is also definitely challenging; some flags took me multiple hours to find as I kept banging my head against a wall. It truly tests virtually everything that you have learned in the course, and you should take it seriously.

I did not do any preparation before starting the exam. I took a four-day break after finishing the coursework, then jumped right in. I had completed two Sherlocks on the main Hack The Box platform prior, but it didn't contribute that much to my success.

## Time and Effort

I started the course on February 8 and completed it on March 15. After a 4-day break, I started the exam on March 19 and submitted the report on March 26, making a total of 44 days spent on the certification. At the time, I was doing the certification alongside a full college workload (12 units). The estimated time duration for the course according to HTB Academy is 23 working days (8 hours per day), and alongside the exam, that puts it at an estimated total of 30 days.

Thirty days is a significant time investment, and as everyone is different, some may take longer or shorter depending on prior experience, the student's learning ability, life stuffs, and other factors. For me, if I wasn't doing college work, I was completing the CDSA course, spending up to 6-8 hours each day. During spring break, I was pulling 12-15 hours per day. I also had no prior blue teaming experience, so I had to take time to understand the concepts taught. But of course, your experience may differ from mine.

## Tips

For the course:
- **Take good notes.** This is a no-brainer, but taking good notes will help retain knowledge of content and it serves as a handy reference when you need it. Whatever notetaking style helps you with retaining knowledge, do it. I am terrible at taking notes; mine are basically a rewrite of the entire modules.
- **Take breaks when necessary.** There is a lot of content packed within 15 modules, and it is very easy to get burnout. Don't be like me where I spent every possible moment working on the course; I'm paying for it dearly.
- **Have a firm understanding of the content.** It is essential to understand exactly what you are doing and why you are doing it. The exercises and the exam will test your understanding, not to mention that the skills you learn are meant to be applied in real-world scenarios. If you are struggling on a particular topic, you can always do some research or ask for pointers in the HTB Discord.

For the exam:
- **Have good documentation.** This is an extension of taking good notes, and having good documentation will make reporting much easier. Write down all SIEM queries and IOCs, grab screenshots for evidence, and have a skeleton technical analysis laid out that you can translate into your report.
- **Utilize HTB Academy's search feature.** If you need a reference for a particular topic that you don't have in your notes, you can use the search bar in HTB Academy to find what you are looking for. Very handy to have, and saves a lot of time.
- **Understand that you will not find everything.** Much like a real-world security incident, you will not have a complete understanding of the nature of the attack. It is best to report everything that you are confident of and provide ample evidence to back up your claims.
- **Never give up.** You have gotten this far. You've completed the course; you are more than capable of completing the exam. Keep going at it, and you will eventually find what you are looking for.

## FAQ

> How should I prepare for the exam?

The course is all you need to pass the exam. I was able to pass without doing any preparation at all since the course acts as preparation.

> How do Sherlocks compare to the exam?

The exam is a vastly different experience from Sherlocks, and most of what you will find in Sherlocks are out-of-scope for the exam. You can do them to develop your methodology, but do not expect them to be anything close to the exam environment.

> Should I take time off to do the exam?

This is entirely up to you, and it will depend on how comfortable you are with the course content. I didn't have the luxury of doing so, but I was still able to complete the exam. As it is 7 days long, you may find it beneficial to do so.

> How does CDSA stack up with other similar hands-on certifications or courses? (BTL1, CCD, etc.)

I have no knowledge of the content of these certifications or courses, so I cannot give an accurate answer.

> Can CDSA land me a job?

No certification can guarantee you a job. Since CDSA is so new, not many job listings, if not none, are looking for this certification, much like CPTS. However, the course content arms you with the skills needed to adequately perform a SOC analyst's job duties.

> Do I need prior experience to complete the course?

No. The course is designed to teach you everything from the basics to intermediate-level skills. If you are a newcomer to cybersecurity, I recommend completing both the Information Security Foundations path (completely free) and the SOC Analyst Prerequisites path. These two paths should equip you with everything you need to complete the CDSA course.

> Are you copying Xre0uS?

Yes, because [his blog post](https://xre0us.io/posts/cpts-oscp-and-you/) is so damn well written.
