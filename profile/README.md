# MeetPlan

<img src="https://avatars.githubusercontent.com/u/81251558?s=200&v=4" align="right" alt="MeetPlan logo">

MeetPlan is a student information system (shortly SIS). It's fully open-source, extremely customizable, with [backend](https://github.com/MeetPlan/MeetPlanBackend) written in Go & [frontend](https://github.com/MeetPlan/MeetPlanFrontend) in Svelte. Deployment is extremely easy using [Docker](https://github.com/MeetPlan/MeetPlanDocker). It uses our internal library, called Proton, which is a fully open-source library, that manages your substitutions & soon even creates timetables for you.

We have some really powerful tools, such as documentation exports (certificates of ending grades, certificates of schooling), meal ordering and much more. Try it, you won't regret it (though it's only in Slovenian, which I agree, is a problem, but this system is currently targeted at Slovenian audience & schools).

## Demo
Demonstration server is publicily available at https://meetplan.meetplan.ml. It will be hosted until my educational resources run out (in about 6 months as of May 9th 2022). These servers are provided for educational purposes ONLY and shall not be misused. The author has right to pull away the server hosting at any time.

Usernames and passwords. Be sure to use them how they are intended for use, otherwise, they WILL BE REVOKED. None of these accounts feature administrator access to the system.

Role: `student` <br>
E-Mail: `student@meetplan.ml` <br>
Password: `student`

Role: `parent` <br>
E-Mail: `parent@meetplan.ml` <br>
Password: `parent` <br>
Parent of: `student@meetplan.ml`

Role: `teacher` <br>
E-Mail: `teacher@meetplan.ml` <br>
Password: `teacher`

## Installation
Our guide on installing MeetPlan to a virtual machine is really extensive & beginner-friendly. It's recommended to follow this guide, as it's the only one officially tested.

[English](https://github.com/MeetPlan/MeetPlanDocker/blob/main/INSTALLATION_en.md)

## Desktop app
![image](https://user-images.githubusercontent.com/52399966/167269792-e58dfa23-33c9-4b82-bd50-9c26b57328ac.png)
*MeetPlan Linux app running on Fedora*

Recently, we adopted [Tauri](https://tauri.studio/), which is a cross-platform framework for building JavaScript apps. Basically, it's our webapp packaged into Windows installation files (.msi), Debian (Linux) packages (.deb), Linux AppImages (.AppImage), MacOS packages (.dmg) and MacOS tarball (.tar.gz). Mobile support is not yet here for Tauri, but when it comes out, we'll also package it for Android & iOS. This app is currently in early alpha, but most features are working. App is available for download on [releases](https://github.com/MeetPlan/MeetPlanFrontend/releases) page of [MeetPlanFrontend](https://github.com/MeetPlan/MeetPlanFrontend). Note, that last release isn't always latest. Be sure to download stable release. Nightly releases are marked as prereleases.

If you are using [Docker configuration](https://github.com/MeetPlan/MeetPlanDocker), the URL you enter on login page is protocol (`https://` or `http://`), your domain and `/api`. Example: `https://example.com/api`

## Overview with timetable
![image](https://user-images.githubusercontent.com/52399966/165902146-a281d35f-41e5-40b5-9c07-4d5727a2cf9e.png)

## Roles
Our system has a lot of roles, some are under ongoing implementation. Our roadmap is visible [here](https://github.com/orgs/MeetPlan/projects/3/views/1?sortedBy%5Bdirection%5D=desc&sortedBy%5BcolumnId%5D=Status). Currently implemented or work-in-progress roles are (by permissions):
- [x] Admin
- [x] Principal
- [x] Principal assistant
- [x] School psychologist
- [x] Food organizer
- [x] Teacher
- [x] Parent
- [x] Student

## Special features
Our system also has a lot of special functions:
- [x] Timetable management
- [x] Proton
- [x] Meals
- [x] Communication
- [x] Absence management
- [x] Homework management
- [x] Grades
- [x] Gradings
- [x] Student & Parent overview
- [x] Realization with a pie chart
- [x] Exports of different documents (class ending certificate (spričevalo) & certificate of schooling (potrdilo o šolanju))
- [x] Desktop app
- [ ] Mobile app (coming soon)

Even more things are currently planned, from expanding Proton, to simple bugfixes, so [stay tuned by visiting MeetPlan roadmap](https://github.com/orgs/MeetPlan/projects/3/views/1?sortedBy%5Bdirection%5D=desc&sortedBy%5BcolumnId%5D=Status).

## Showcase
### Meeting details
![image](https://user-images.githubusercontent.com/52399966/165902179-e28ea67e-f11a-4474-8356-c8f4536e41b6.png)

### Substitution management - make your life easier with Proton
![image](https://user-images.githubusercontent.com/52399966/167196652-3ad43bd4-441b-4464-8bef-80d57f3daffd.png)

### Absence management
![image](https://user-images.githubusercontent.com/52399966/165902218-ec830d27-1e5b-4e8d-b6ef-41147f63eb7d.png)

### Grade management
![image](https://user-images.githubusercontent.com/52399966/165902267-d4b042a8-ad4c-4584-a4bc-ac0a06175e7b.png)

### Homework management
![image](https://user-images.githubusercontent.com/52399966/165902323-a37f0952-1022-4c97-b490-8e507fd60f26.png)

### My overview - Student can view it's own information - grades, absences, homeworks & gradings. Data should serve you, not companies.
![image](https://user-images.githubusercontent.com/52399966/165901293-db19e876-c300-4868-98f7-619372227109.png)

### Class teacher student overview
![image](https://user-images.githubusercontent.com/52399966/165902421-adae49fc-0b13-44f6-be15-5a37bd2e5546.png)

### Communication - be in touch with teachers & other school staff - supports Markdown
![image](https://user-images.githubusercontent.com/52399966/165901812-36511a7f-1ea7-40fb-98fe-9d30ea47ae3b.png)
![image](https://user-images.githubusercontent.com/52399966/165901887-0433e8cd-f19a-4cbe-bdb7-6bab7f5d7544.png)

### Meals - order meals with ease
![image](https://user-images.githubusercontent.com/52399966/165902025-cc16115f-8c8b-4fcf-af72-9faf28011bc2.png)

## Full disclaimer (legal stuff)
Most of the code under this organization is licensed under AGPLv3 license, but you have to check the coresponding repository for a license. Code can be freely used even in other projects under the statements and copyrights provided by the license. All the code in the repository is licensed under one specific license UNLESS it's explicitly defined otherwise.

MeetPlan was designed to be a replacement to [eAsistent](https://easistent.com) and [Lo.Polis](https://www.lopolis.si/), which are both outdated and extremely pricey/costly. Both of these Student Information Systems can generate certificates and official documents, as it's a useful feature to schools, that saves a lot of time. MeetPlan is an educational project and SHALL NOT BE MISUSED IN ANY WAY. The author, contributors and the MeetPlan Team don't allow any misuse of the software, such as forgery of official documents. Author, contributors and the MeetPlan Team SHALL NOT IN ANY WAY BE LIABLE FOR MISUSE OF THIS SOFTWARE. You and solely you are liable on what you do with this software. You have been warned.
