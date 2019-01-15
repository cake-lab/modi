---
title: "MODI: Mobile Deep Inference Made Efficient by Edge Computing"
authors: Samuel S. Ogden and Tian Guo
authors_list: 
  - sam
  - tian
pdf_location: https://www.usenix.org/system/files/conference/hotedge18/hotedge18-papers-ogden.pdf
journal: The USENIX Workshop on Hot Topics in Edge Computing (HotEdge ‘18)
excerpt_separator: <!--more-->
publication_date: 07-10-2018

layout: publication
---

In this paper, we propose a novel mobile deep inference platform, MODI, that delivers good inference performance. <!--more--> MODI improves deep learning powered mobile applications performance with optimizations in three complementary aspects. First, MODI provides a number of models and dynamically selects the best one during runtime. Second, MODI extends the set of models each mobile application can use by storing high quality models at the edge servers. Third, MODI manages a centralized model repository and periodically updates models at edge locations, ensuring up-to-date models for mobile applications without incurring high network latency. Our evaluation demonstrates the feasibility of trading off inference accuracy for improved inference speed, as well as the acceptable performance of edge-based inference.