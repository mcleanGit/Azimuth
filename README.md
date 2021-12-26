README.md
# Code Refactor Starter Code
# 01 HTML, CSS, and Git: Code Refactor
# Repository: mcleanGit/Azimuth
# Horiseon Brand Optimization Management Marketing

## Brief Description

The project responds to a request from the Horiseon marketing agency for a code refactor that will render its site ==more accessible== so that it is ==optimized for search engines==. These issues are at the forefront of many digital media discussions today. Since, in providing services for their own clients, the core business of the agency is also centered on these matters, the business need for improvement is mission critical.

*Motivation.* As an executive leader for many years in higher-education and innovation in the performing arts and digital media, I am driven by the socio-economic, organizational, and technological impact of these transformative fields. Now that my institutional administrative role is completed, I am reengaged in many ongoing projects in interdisciplinary research and infrastructure development. In addition to their legacy value, some of those projects also explore new horizons, in part related to my role as co-founder of Digital Media at the Crossroads (DM@X) and other networking initiatives. I am motivated to expand my circle of influence and range of capability by working from the ground up, to explore the coding and implementation aspects of the digital present and future as an important complement to my executive experience in these areas.

*The client*. The client is a marketing agency specializing in digital branding. The name Horiseon modifies horizon to embeds ==seo== (Search Engine Optimization), which is one of the three main services provided. The others are Online Reputation Management and Social Media Marketing. Other business features include: Lead Generation (initiation of customer interest), Brand Awareness (increasing search ranking and visibility), and Cost Management (increased search ranking can decrease advertising costs).

*The project.* The client webpage mockup is reasonably attractive and functional. It would form the basis for further discussion of the development of more compelling UX/UD user experience. At present, however, the source code reveals a number of inefficiencies and superannuated norms that can be refactored to improve what I would call ==internal==, as well as ==external== accessibility (as discussed further below).

*Proposed title.* Horiseon Brand Optimization Management Marketing

*SEO and Title.* As Horiseon is a company offering search engine optimization for its clients, it is imperative that its own seo models success. Since the title line in the head of the HTML code is a fundamental keyword element for Google and other search engines, the proposed webpage title is: Horiseon Brand Optimization Management Marketing. This title captures the key components of Horiseon services, including the company name, its ultimate focus on Brand, and the component elements of search engine Optimization, online reputation Management, and social media Marketing. The proposed title might be revisited in subsequent discussions with the client and following some user analytics.

*Accessibility-External.* The client seeks a codebase refactoring that follows ==accessibility standards== so that their own site improves its ==seo==. Accessibility is a complex and currently high-profile consideration for most organizations. Aspects of accessibility are government mandated; for example, the Province of Ontario (https://www.ontario.ca/page/accessibility-in-ontario) has established legislation (AODA 2005) and guidelines for website accessibility and all commercial websites (https://www.ontario.ca/page/how-make-websites-accessible) were expected to be compliant as of January 2021. Some aspects of the AODA requirements are indirectly addressed in this Code Refactor for Horiseon. These elements might be understood as ==external== aspects of accessibility.

*Accessibility-Internal.* There are also ==internal== ways to improve the accessibility of the Horiseon website/webpage. Although such improvements are partly realized in the URL implementation of the refactored code, the intention at this stage is that the basic functionality and mockup remain largely unchanged. However, the source code currently reveals a number of inefficiencies and inconsistencies that affect its internal accessibility and future sustainability for the IT support team. For example, the source code for the webpage diminishes clarity in its limited use of standard HTML semantic elements, shows lapses in logical structuring and related styling and positioning of code, and lacks the now-requisite alt descriptions for images. These issues are further addressed in a brief overview of Refactored Elements, next.

*Refactored Elements.*
The source code/page was tested for links. All were functional with exception of nav link to the first seo anchor, as noted below.

*HTML semantics.* The source code overuses the now-often-superseded div for all divisions of the page. For future code team accessibility (legibility) and sustainability (anticipating further site growth), several divs were changed to employ semantic HTML norms: nav, header, and footer. Others are possible, but not yet implemented at this stage; e.g., the use of section for the main content and possibly aside for right-hand the sidebar if this benefits div is felt best construed with that function.

*CSS-HTML matching.* The relevant CSS stylesheet was changed to match the HTML, replacing several .class calls with semantic calls. This consolidation of CSS selectors and properties involved changes to both parent and inherited elements; for example, in the multiple styles associated with the original class .header (in its change to semantic header).

*Nav.* Navigation clarity was improved in the header section by replacing the generic div of the unordered list of anchor elements within nav. As noted above, the first anchor link to Search Engine Optimization section/div of the page was not functioning; due to the omission of its id=… Fixed.

*Alt.* For accessibility expectations, alt attributes were provided for the image elements. Images in the main content section were given alt attributes. The benefits section uses three png icons (lead, brand, cost), rather than photographic images. These typically do not expect alt attributes but could emerge as a need in further discussions with the client. See next paragraph for hero alt exception.

*Hero element.* The main hero/jumbotron div uses a background-image, often found in the CSS (as is the case here) rather than in the HTML. There is no further content. Such background-images do not typically require alt entries. However, if the client, in further discussion, feels that the prominent image conveys content (the dynamic team, for example), it should be changed to an img in the HTML with an appropriate alt. There is an alt workaround for background-images, called an aria-label, which was added to the HTML in its current form. 

*Font-size.* Minimum font-size expectations for AODA compliance is 16px, which is the generic p provided. It was worth experimenting to see if some of the p attributes could be given larger font-sizes in some places, without skewing the basic mockup. Font-size for .content p in the three main content boxes was increased to 20px, improving ease of reading for some disability constituencies. The p for the benefits sidebar needed to remain at 16px to avoid skewing the current layout.

*Grouping of CSS elements.* CSS elements were reorganized to follow HTML semantic structure. It would be possible to group more of the CSS selectors that have the same properties and values. For example, the three content boxes and the three benefits icons have consistent declarations in their container, img, and h selectors. They could (with some caveats) be rolled up to the parent element to save lines of code. However, at this point in the project, it was felt better to leave the divisions (and subdivisions) distinct (even though code repetitive) to foster further consideration of possible variations.

End of README.md


