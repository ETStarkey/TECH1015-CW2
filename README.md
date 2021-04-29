# TECH1015-CW2
TECH1015-CW2 Submission

**Title**: Portfolio Webpage
------------

---

**Concept**: A portfolio website to showcase a range of my creative works, from fine art, to digital media that functions over a variety of devices (widescreen, mobile, tablet, standard PC, etc.).
------------

*Utilising a tab system (using JavaScript to show and hide content divisions as needed) to catagorise different mediums of work from one-another, one tab focused on my fine art using various images to display examples of my previous artworks, another tab for my digital medium of work, another using video(s) (of suitable resolution for deployment) for my own video projects - Time (and suitable placement) permitting, I may be inclined to add a contact section for feedback or to get in contact with me.*

- Tabbed system to catagorise work mediums
- Be mindful the site still somewhat functions without becoming unusable if JavaScript is not enabled, as an example; this can be achieved (I believe) by structuring the site to work as a standard scrolling site, and then using divs+JS to hide/display the correct content as needed, this content could possibly begin to add onto the load times of the site also, which I will keep an eye on in testing as Firefox has a great tool for measuring load speed over average mobile data plan speeds AND tools for testing mobile features/adaption.

---

**.**:

I will be beginning with what I believe to be the "standard" html set-up, an index.html page to act as a landing page for anyone visiting the site, for this case I will just be using this one page for my site and use JavaScript to give the illusion of different webpages, this should (hopefully) remove loading inbetween browsing on the site, with the majority of content being downloaded in advance (permitting that it is not a rediculous amount of data, so automatic videos or animated backgrounds are probably worth avoiding if not scaled accordingly).

![Standard HTML Setup](./img/readme-img/standardHTMLSetup.png)


I want this site to be reflective of myself, the work I produce, and ideally a general aesthetic that isn't oversaturated with animated images or backgrounds that take away from the contents of the portfolio, but instead can compliment and highlight the portfolio's content.

I have previously experimented with works that utilised a gif background for mobile viewports, but a full-scale 1080p video for PC browsers, though this seems excessive as previously expressed. Perhaps though, the gif background, or more specifically a similar effect of light animation in the way of emulating the effect of a CRT monitor could be worth investigating.

---

**Testing the first commit**:
------------

Interestingly enough, while trying to get my first commit of the site up to have a skeleton to work with and build on, when I first loaded the GitHub page, nothing showed but a black screen.

![Black screen faced after first commit](./img/readme-img/blankFirstCommit.png)

This struck me as odd, so I used Firefox's troubleshooting skill to locate a silly but common error:

![Blocked Content Error](./img/readme-img/BlockedContentError.png)

It turns out that two scripts were being blocked by Firefox because the portfolio site would load HTTPS, while these script links were HTTP - no S.
"Starting in Firefox 23, mixed active content is blocked by default."; this prevented the "Loader" script that would hide our .se-pre-con class cover for the site was not working as intended, and wouldn't reveal the site.

![Small commit adding HTTPS links for scripts](./img/readme-img/HTTPSCommitFix.png)

[After this small commit](https://github.com/ETStarkey/TECH1015-CW2/commit/f1cd13e86ad174b7d0e48af91d3695cf37418f2b), the problem has been resolved, and the script works as intended, revealing the site after a fast load.

![State of fixed site on GitHub Pages](./img/readme-img/postFixSite.png)


------------
