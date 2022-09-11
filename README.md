# Joomla! SEO Project | GSoC 2022

![GSoC2022-AlishaKamat-](https://user-images.githubusercontent.com/84401192/189527186-05234942-7e24-4d49-9b99-7566ae28a8bd.png)

## Introduction
<b>Initial Project Workplan:</b> [Initial Workplan Link](https://docs.google.com/document/d/14N_4oAD4ZLIfuPH0T9GaAHSIE8pOGd00uEMdayuhonE/edit)<br>
<b>Project Repository:</b> [Repo Link](https://github.com/joomla-projects/gsoc22_seo)<br>
<b>Weekly Reports:</b> [Reports Link](https://volunteers.joomla.org/teams/gsoc-2022-seo#reports)<br>
<b>Joomla CMS Repository:</b> [Repo Link](https://github.com/joomla/joomla-cms)<br>

Core features covers 9 tasks:
<ol>
  <li>New SEO tab</li>
  <li>Dofollow / Nofollow checker for outgoing links</li>
  <li>Performance check on PageSpeed Insights</li>
  <li>Paragraph structure</li>
  <li>Sentence Structure</li>
  <li>Content analysis</li>
  <li>Reading ease rating [Flesch Kincaid]</li>
  <li>Adding open graph data</li>
  <li>Article Image Compression</li>
</ol>


Bonus tasks include:
- Social Media Share buttons (added to Joomla core)
- Content Analysis Plugin
- Open Graph Plugin
- Previews Plugin
- Meta data Plugin


## Pull Requests
S.No. | Task | Project Repository PR
--- | --- | ---
1 | SEO Tab | [PR #1](https://github.com/joomla-projects/gsoc22_seo/pull/1)
2 | Nofollow-Dofollow Link checker | [PR #3](https://github.com/joomla-projects/gsoc22_seo/pull/3)
3 | Page Performance Analyser | [PR #4](https://github.com/joomla-projects/gsoc22_seo/pull/4)
4 | Paragraph structure | [PR #5](https://github.com/joomla-projects/gsoc22_seo/pull/5)
5 | Sentence Structure | [PR #6](https://github.com/joomla-projects/gsoc22_seo/pull/6)
6 | Google SERP preview and Content Analysis | [PR #7](https://github.com/joomla-projects/gsoc22_seo/pull/7)
7 | Reading Ease Rating | [PR #8](https://github.com/joomla-projects/gsoc22_seo/pull/8)
8 | Open Graph | [PR #9](https://github.com/joomla-projects/gsoc22_seo/pull/9)
9 | Image Compression | [PR #14](https://github.com/joomla-projects/gsoc22_seo/pull/14)
10 | Social Media Share buttons | [PR #15](https://github.com/joomla-projects/gsoc22_seo/pull/15)

## Plugins
S.No. | Task | Link to Plugin
--- | --- | ---
1 | Content Analysis Plugin | [Link #1](https://github.com/joomla-projects/gsoc22_seo/tree/content-analysis-plugin)
2 | Open Graph Plugin | [Link #2](https://github.com/joomla-projects/gsoc22_seo/tree/opengraph)
3 | Previews Plugin | [Link #3](https://github.com/joomla-projects/gsoc22_seo/tree/preview)
4 | Meta data Plugin | [Link #4](https://github.com/joomla-projects/gsoc22_seo/tree/metadata)

<hr>

## Core Features
### Google SERP Preview
This new feature gives Joomla content creators an idea of how their article will appear to the end users on search engines. It becomes extremely important for the content creator to customize this piece of information as there is limited space available.<br>
It can also be thought of as a small advertisement for the Joomla user’s content to attract potential leads.

### Content Analysis
This feature is related to the previous feature (SERP Preview). It highlights the aspects of the article that need improvement and also provides suggestions for refinement. Some of these parameters include the article title, meta description, and article word count. Fixing these can boost the article’s click rate significantly.

### Page Performance
A simple way to measure the page’s core web vitals with a single click. It provides insights on the page’s loading speed and ratings for the article based on multiple criteria while also providing suggestions to fix the issues.

### Outgoing Dofollow-Nofollow Link Checker
This allows the admin to monitor the external links of the article and categorize them as dofollow and nofollow. It will enable developers to prevent ‘link juice’ from flowing out to unwanted sites based on the external site's credibility. Admins can choose to retain or change the ‘rel’ directive (from dofollow to nofollow or vice versa) by going to the 'Content' tab on the same page. They can even choose to remove the link altogether.

### Readability Rating [Flesch Kincaid]
This feature provides a rating based on the article’s difficulty level. It also highlights where the rating falls in the difficulty range. Rather than simply relying on a rating, the target audience should also be considered before making changes.
For instance, an academic article may typically have a lower rating (a significantly high difficulty level for average readers) but the target audience (university grads) won’t find it too difficult to comprehend.

### Paragraph structure
Having a concise paragraph structure is ideal for SEO and also improves the article's readability especially on smaller screens. Nowadays, people prefer audio/video content over text content. Attention spans are dropping. This makes it crucial for text content creators to capture the reader’s attention. One way to do that is by including crisp and short paragraphs as opposed to long and tedious ones that are difficult to read.
Having an ideal paragraph structure improves an article's discoverability on search engines. This feature assists in keeping article paragraphs short and easy to read for viewers. It lists down the top 5 paragraphs that exceed the word limit along with the word count in brackets. Currently the limit for each paragraph has been set to a maximum of 200 words
 
### Sentence Structure
This works similar to the previous feature with the difference that it works for sentences as opposed to paragraphs.
This feature helps identify the first 5 sentences that are too long to avoid clutter and lists them. The admin can then switch to the Content tab and make the desired changes. Currently the limit for each sentence has been set to a maximum of 20 words
 
### Image Compression
Images are among the biggest ‘on-page’ factors for a slow loading page. This new feature helps compress large, unoptimized images to improve the page load time.
Currently the proof of concept works for
The image fields under the Images and Links tab in Article Edit view
Two formats, 'png' and 'jpeg'
The compression feature is optional (controlled using the enable/disable toggle) and gets triggered when the user saves the article. For a successful compression operation, it also stores a backup of the original image as filename_orig.
It provides the user with 3 compression options
- Low Compression - High quality
- Medium Compression - Medium quality
- High Compression - Low quality

### Open Graph
It gives Joomla content creators the ability to customize their article previews when it’s being shared on social networking sites. It provides users the flexibility to modify each article's open graph data, which in turn can be used by social media platforms to display rich objects. Some of these parameters include
Article Type
Article Title
Article Description
Article Image
Published Date
Article Author

<hr>

## Mentors
Thank you to 
1. Elisa Foltyn
2. Phil Walton
3. Benjamin Trenkle

Special Thanks to Richard Fath and Christiane Maier-Stadther <br>
Also also to my fellow GSoC student contributors - [Shazma Siddiqui](https://github.com/shazmasiddiqui), [Khushi Rauniyar](https://github.com/khu5h1) and [Shubham Verma](https://github.com/Shubhamverma2796)

<hr>

## Future Roadmap

