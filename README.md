# From CSSE to Backend Engineer: A Graduation Learning Plan

**Prepared for:** Husky student pursuing a job as a backend software engineer  
**Prepared by:** Slavik Arushanyan  
**Date:** November 5, 2026

© 2026 Slavik Arushanyan

---

**Table of Contents**

- [Purpose](#purpose)
- [Best Practices](#best-practices)
  - [Taking backend electives in order](#taking-backend-electives-in-order)
  - [Deploying and measuring a backend service](#deploying-and-measuring-a-backend-service)
  - [Contributing to open source projects](#contributing-to-open-source-projects)
- [References](#references)

---

# Purpose

Most of what the CSSE core teaches you is how to write correct code. Backend job postings ask for more than that. GitLab's backend roles, for example, require experience fixing performance problems, clear technical communication, and the ability to work on a remote team, and none of those get much attention in core classes.[^1] This plan covers three things to do between junior year and graduation: take backend electives in the right order, deploy a service and measure how it performs, and contribute to an open-source project. Figure 1 shows when each one happens. The purpose of this plan is to get you to graduation with backend work you can point to on your resume and in interviews.

---

# Best Practices

The order matters. The electives come first because the project depends on them, and open source goes better once you have some backend experience.

## Taking backend electives in order

Backend engineers mostly work on the parts of an app that users don't see, like databases, APIs (application programming interfaces), and the servers in between. The core covers data structures and algorithms well, but it doesn't really get into databases, networking, or cloud systems, and that's most of what backend work runs on. Kleppmann describes the main goals of a data system as keeping it reliable, scalable, and maintainable,[^2] and all of those depend on how databases and networks behave. Timing is the other issue. Some of these electives have prerequisites, and CSS 436 is only offered in winter and spring.[^3]

**Take CSS 430 Operating Systems and CSS 475 Database Systems in junior year, then CSS 432 Network Design and Programming, and leave CSS 436 Cloud Computing for senior winter.** CSS 430 is recommended before CSS 432, and CSS 436 requires one of the two.[^3] While you take each class, add one small piece to a personal server project. For example, build the database layer during CSS 475 and the REST API during CSS 432. If a class fills up, Figure 1 shows a backup quarter for it.

**Figure 1.** *Backend learning timeline from junior fall to senior spring, with recruiting season shaded*
 
![Gantt-style timeline from junior fall to senior spring with three lanes: Courses, Projects, and Experience. Fall quarters are shaded as recruiting season. Arrows connect each elective to the project feature it enables, diamonds mark milestones like the service going live and two merged pull requests, and dashed bars show backup quarters for full classes.](images/figure1-timeline.png)

## Deploying and measuring a backend service

A personal or class project usually runs on your laptop with one person using it, so you never find out where it would break under real use. Diagnosing performance problems is listed as a requirement for every backend role at GitLab.[^1] Google's *Site Reliability Engineering* book recommends watching four "golden signals" on a live service: latency (how long a request takes), traffic, errors, and saturation (how close the system is to full).[^4] Those numbers only mean something once a service is deployed.

**By the end of junior year, deploy one service with a database to a cloud host and load test it.** Load testing is sending heavy simulated traffic to see when it slows down. While you do this, track the four golden signals, find the biggest bottleneck, and fix it. After that, write a one-page design doc, which is a short write-up of what you built and the tradeoff decisions that you decided to make. GitLab lists clear technical communication as a requirement too,[^1] so the doc is worth the extra hour. Get all of these steps done before senior fall, as that's when full-time recruiting starts (see Figure 1).

## Contributing to open source projects

GitLab lists open-source experience and developer tools as nice-to-haves for backend engineers, and it requires being able to work on a remote team that mostly communicates asynchronously.[^1] An open-source project covers both, and since you work in a codebase much bigger than anything from class, you use the project's Git and CI (continuous integration) setup, and people you have never met review your code in writing. Many students don't get that kind of review until their first internship, and that's why it is beneficial to do.

**Get at least two small PRs (pull requests) merged in a backend or developer-tools project before senior fall.** Start with something small like a typo or docs fix, and make sure to read the CONTRIBUTING file first.[^5] After you get comfortable, open an issue first for bigger changes.[^5] The Git workflow from CSS 360 covers most of the basics you need here.

---

# References

[1] GitLab, "Backend Engineering Roles," *The GitLab Handbook*, n.d. [Online]. Available: https://handbook.gitlab.com/job-description-library/engineering/development/backend/. [Accessed Oct. 26, 2026].

[2] M. Kleppmann, *Designing Data-Intensive Applications*. Sebastopol, CA, USA: O'Reilly Media, 2017.

[3] University of Washington Bothell, "Computing and Software Systems," *UW Course Descriptions*, n.d. [Online]. Available: https://www.washington.edu/students/crscatb/css.html. [Accessed Oct. 26, 2026].


[4] R. Ewaschuk, "Monitoring Distributed Systems," in *Site Reliability Engineering*, B. Beyer, C. Jones, J. Petoff, and N. R. Murphy, Eds. Sebastopol, CA, USA: O'Reilly Media, 2016, ch. 6. [Online]. Available: https://sre.google/sre-book/monitoring-distributed-systems/. [Accessed Oct. 26, 2026].

[5] Open Source Guides, "How to Contribute to Open Source," *Open Source Guides*, n.d. [Online]. Available: https://opensource.guide/how-to-contribute/. [Accessed Oct. 26, 2026].

[word count: 688]

[↑ Back to top](#from-csse-to-backend-engineer-a-graduation-learning-plan)

[^1]: GitLab, "Backend Engineering Roles," *The GitLab Handbook*, n.d.
[^2]: M. Kleppmann, *Designing Data-Intensive Applications*, 2017.
[^3]: University of Washington Bothell, "Computing and Software Systems," *UW Course Descriptions*, n.d.
[^4]: R. Ewaschuk, "Monitoring Distributed Systems," in *Site Reliability Engineering*, 2016.
[^5]: Open Source Guides, "How to Contribute to Open Source," n.d.


