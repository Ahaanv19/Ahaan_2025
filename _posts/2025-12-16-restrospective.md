---
layout: post
title: Personal Highlights, Retrospective Sprint 4
permalink: /retrospective/
toc: true
comments: true
---

# Project Retrospective: Sprint 4

## Project Context and Purpose
The objective was to design and implement an accessibility and user preferences system for our teacher’s website, with the intention of improving how students interact with course materials.

The teacher’s website is used by students across multiple computer science courses, including AP CSA and AP Computer Science Principles (AP CSP). Because the site serves a diverse group of learners with different language backgrounds, learning styles, and accessibility needs, our team focused on creating a system that would make the website more inclusive, adaptable, and supportive for all students.

---

## Team Collaboration and Roles
Working in a team required consistent coordination, shared responsibility, and clear communication. Each team member contributed to different aspects of the project, including planning, design, implementation, and testing.

My primary contributions focused on designing and implementing the preferences and accessibility features, particularly the translation system, text-to-speech functionality, and visual customization options. I also contributed to discussions about system architecture and maintainability, especially around consolidating styles using SASS.

This team-based structure reinforced the importance of dividing tasks effectively while maintaining a shared understanding of the overall system.

---

## Design History and Development Process
The project followed an intentional design progression that allowed us to move from abstract ideas to a functional working prototype.

We began by identifying key challenges students face when using the teacher’s website, such as difficulty reading dense text, navigating content efficiently, and understanding material due to language barriers. Early design work focused on outlining how accessibility features could be integrated without disrupting the existing structure of the site.

As the project progressed, our designs became more detailed, specifying how user preferences would be applied across pages and how different features would interact. This stage allowed us to refine our ideas and gather feedback before full implementation.

Eventually, the project reached the working prototype stage, where all major features were functional and integrated into the website. At this point, the system closely resembled how it would function in a real classroom setting.

---

## Core Features and Technical Implementation

### Visual Preferences and Customization
The system allows students to customize text color, font family, font size, background color, and highlight color. These features help improve readability, reduce eye strain, and support different learning preferences.

By giving students control over the interface, the system removes unnecessary obstacles and allows them to focus on understanding the content rather than struggling with presentation.

---

### Preset Themes
To make customization more accessible, we implemented preset themes such as light mode, dark mode, and high-contrast mode. These themes provide quick, effective configurations for students who want immediate accessibility without manually adjusting individual settings.

---

### Translation Feature and Language Support
One of the most impactful components of the project was the translation feature. This tool was designed to help students who struggle with English better understand content on the teacher’s website.

The translation feature was especially beneficial for **AP CSP students**, many of whom relied heavily on translated explanations to understand instructions and concepts. Students who preferred learning in **Chinese** were able to engage more confidently with the material, reducing reliance on external help and increasing independence.

---

### Text-to-Speech Functionality
The text-to-speech feature allows students to listen to website content rather than only reading it. This supports auditory learners and students who benefit from hearing information presented aloud.

By offering multiple ways to consume content, the system aligns with inclusive learning principles and helps accommodate diverse learning styles.

---

### SASS Consolidation and Maintainability
From a technical standpoint, our team prioritized maintainability and scalability. We consolidated styling using SASS, organizing shared variables, mixins, and theme definitions to reduce redundancy.

This approach made the system easier to update and extend, ensuring that new themes or preference options could be added without rewriting large portions of the codebase.

---

## Impact on Students and Courses
The accessibility system had a meaningful impact on students using the teacher’s website. Students reported improved readability, reduced frustration, and greater confidence navigating course materials.

The impact was particularly noticeable in **AP CSP**, where the translation feature helped students overcome language barriers that previously limited their participation and understanding. By improving accessibility, the project supported more equitable learning experiences across courses.

---

## Reflection on Teamwork
Working in a team highlighted both strengths and areas for improvement in collaboration. While task division allowed us to work efficiently, there were moments where earlier feedback and more frequent check-ins could have improved alignment.

In future team projects, I would strengthen collaboration by:
- Sharing progress more consistently
- Seeking peer feedback earlier in the development process
- Clarifying responsibilities and deadlines at the outset

These changes would help ensure smoother collaboration and more cohesive outcomes.

---

## Reflection on Communication
This project emphasized the importance of clear communication, both within the team and with stakeholders such as our teacher. Explaining technical features in an understandable way was just as important as implementing them correctly.

Going forward, I plan to improve communication by documenting features more thoroughly, explaining design decisions clearly, and regularly updating collaborators on progress and challenges.

---

## Looking Ahead: The Next Chapter
This project is not a completed endpoint, but part of an ongoing development process. As the teacher continues to use and refine the website, there are opportunities to expand language support, improve accessibility features, and incorporate student feedback.

Continuing to iterate on this system while teaching and supporting other lessons reflects the idea that meaningful projects evolve over time rather than being abandoned once an initial version is complete.

---

## Conclusion
Developing this accessibility and preferences system as part of an AP CSA team demonstrated the real-world impact that thoughtful software design can have in education. By focusing on inclusivity, collaboration, and maintainability, the project improved how students interact with the teacher’s website and reinforced the importance of building technology that serves diverse users.

