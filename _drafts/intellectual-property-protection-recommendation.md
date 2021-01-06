---
layout: post
title: Intellectual Property Protection Recommendation
subtitle: ''
date: 2021-01-31 08:00:00 +0000
thumb_img_path: ''
content_img_path: ''
excerpt: Revamping the recommendation experience when customers say, "Help me decide"
hide_header: false

---
# Background

* Broadly, our research has shown people want quizzes or recommendation wizards to narrow down the different legal services they may need.
* For Intellectual Property (IP) LegalZoom has a simple 1-question “Help me decide'' tool on the IP Category page. Testing participants would often be excited to see the tool, but find the actual experience and recommendations disappointing.
* This work was done in concert with a case study project for [Smashing Magazine Behavioral Design Workshop](https://smashingconf.com/online-workshops/workshops/susan-guthrie-weinschenk) (highly recommended!)

## Goals & Requirements

### Target Audiences

* **Small business owners:** protect their business name and products, be legally compliant, and set up their business correctly
* **Musicians & writers:** protect their songs, scripts, books, etc. and prevent others from copying or profiting off their work
* **Inventors:** claim their new product, invest in protecting their work now, for future benefits/gains

### Company

* Customer understands the product offering and **purchases the correct service** for their needs
* Customer is able to purchase & complete their application **without Customer Care assistance**
* Customer **purchases Attorney Assist** if they have any unanswered legal questions

### Redesign Constraints

* Conserve dev resources. Aim for copy and image changes.
* Design for future design system compliance
* Fix any large problems - identify “no regrets” changes
* Include the new product, Attorney Led Trademark

## The Original Experience

### Behavioral Design Workshop Evaluation

* Currently have to choose from an unordered group of 9 items
* Studies have shown people make decisions easier when there are less choices
* It’s difficult to predict content when there is no order
* Icons have inconsistent levels of complexity. The more complicated icons are too difficult to break down into geons, which would allow customer brains to recognize the icon quicker.
* Conceptual models:
  * Language may not match how customers classify their work.
  * Users expect to see reasoning behind the results. Expect to be aided in decisions. Not all results provide a clear recommendation or a way to decide on a product
  * Pricing and packages and LegalZoom’s role are not clear on results page
  * Do users expect to find out what protection our IP services offer, timelines, and level of effort?

### Data

* Roughly 30% get the “Trademark” result, 15% get “Copyright” result and 14% of people get the combination “Trademark and Copyright” result; the numbers get smaller from there.
  * Either there is less appetite for patents or does the experience suppresses that choice
* About 20% of the traffic clicked back or on the logo to go to the homepage. This tells me they didn’t want to answer the question, “What would you like to protect?” but also didn’t want to leave LegalZoom
  * The options might be too specific (they don’t see exactly what they are trying to protect) or too difficult to understand (what exactly counts as an industrial design?).
  * People also called customer care directly from this page.
* Over 35% of the previous pages were results pages
  * Users don't trust the results and took the quiz again
  * Users were not convinced to click the product CTA on the results page - instead clicked back to return to the quiz and back again to the category page.

# Design Process

### Kickoff Questions

* Are these 9 options representative enough of the things our customers want to protect?
* How would our potential customers classify and sort IP?
* What kind of language do they use?
* What kind of classifications do they expect?
* Where are the potential gaps in the choices we provide?

## Customer Research

1. **Card Sorting.** I picked about 20 commonly protected works from the United States Patent and Trademark Office, various online services, included us, (e.g. photograph, process, book, invention, logo, song) and asked participants to sort the cards into groups and answer a short survey.
   1. **Phase 1: Open**
      * "Art" cards were overwhelmingly the easiest for folks. Second was business - sometimes called “branding”
      * Seeing all the cards in groups helped solidify their classification _(which reminds me of partitioning/the power of groups from the workshop)_
   2. **Phase 2: Hybrid**
      * I provided 3 categories from the Open results. The first two categories were clear winners from the Open Card Sorting, the 3rd was experimental.
      * Works that would require patents emerged as the hardest IP to categorize. (Low patent numbers  site analytics too)
2. **Prototyping.** The team decided to use the questionnaire component of the existing design system. The variations are content-driven.
   1. **Version 1: Optimized**
      * Keep the 1-question flow, but reduce the number of options to broad categories and add descriptions.
      * Hypotheses:
        1. Participants will be more successful if we reduce the number of options. The legal team and copywriters felt comfortable combining the “Art” choices since most of the card sorting participants always grouped those together.
        2. Educating the users with descriptions and friendlier language will clarify the options. The confusing cards from the card sorting study were added as examples in the descriptions.
   2. **Version 2: Experimental**
      * Make a 2-question flow, partition people into roles (business owner, artist, or inventor) and have more specific choices on the second screen.
      * Hypotheses:
        1. If we use nouns to trigger group membership, users will feel more motivated to complete the first question. Adding a second, more meaningful question will improve the inconsequential feeling of the 1-question live experience.
        2. We can reduce errors by utilizing the power of groups/partitioning and encourage people to think more about their selection. This is also an opportunity to add more choices - as card-sorting participants understood IP better when they could see the groups.
3. **Unmoderated Tests.** First round is focused on our largest audience: future small business owners. The pages before and after the “Help me decide” experience - including the results pages were identical. Participants only saw one version and the results from the two studies were compared.
   1. Version 1 participants had a very high NPS score and scored their confidence in the results as 5/5. However, only 3/7 got a recommendation for the correct IP protection
   2. Version 2’s NPS was 30 points lower and an average of 4.6 confidence score. Interestingly, all the participants chose the correct service!!
   3. Our recommendation on the results page isn’t enough to convince people.

### Reflection & Next Steps

I thought these results were wild! We clearly need to tinker and continue to test with both versions.

* How can we reduce the error rate on Version 1?
* What are some other ways we can partition the choices?
* We successfully reduced errors, but how can we increase confidence and improve the experience of Version 2?
* Explore different ways people can validate their results (e.g. articles/faqs, statistics, real-life examples or case studies)

Expand the next round of unmoderated tests to include more audiences. When we get comfortable with the 2 versions, we’ll move on to moderated testing and eventually roll out to development and A/B testing.

In the meantime, for the first phase of the redesign, we started with a logo change and updated the most confusing terms.

* **Timeline:** \~4 weeks in Q3 2020, Phase 2 is scheduled for Q1 2021
* **Team composition:** Copywriter, attorney, product marketer and 2 product designers
* **Role:** Research, Product/UX Design