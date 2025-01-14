# YHS-LibGuide-Customizations
 This a customization project for York House School's Senior Learning Commons LibGuides 2 website.
# To Do...
- Setup safe dev environment
- Styling Ideas
	- Would be nice to move the guide subject list to top of page, for visibility
	- afix nav to top of screen
	- make nav highlight current page https://stackoverflow.com/questions/34491182/make-bootstrap-tab-active-on-the-bases-of-url-link
	- Apply brand colours to site
- Content Ideas
	- Write a friendly intro in the custom template for 
		- A-Z databases
		- Subject & Subject Landing pages
	- 
- Figma implementation
	- Site-wide
		- Style using brand colours
		- navigation bar announcement ribbon
		- Footer
		- sidebar boxes
			- Hours & map
			- Contact us using google form embed
			- toggle visiblity button (visible by default on desktop, hidden by default on mobile)
	- Home page
		- Image hero
		- New post carousel (manually populated?)
	- Guide Page
		- internal guide nav menu on left side

# LibGuide Limitations
- Don't have a way to upload custom fonts - need to use [google hosted fonts](https://fonts.google.com/).
- Can upload custom images
- Can edit individual HTML templates for:
    - Homepage
    - Guides
    - Search Results
    - Subject Page
    - Profile
    - A-Z Guide Browser
- Can edit CSS & JS: Site-wide, or embed in per-page `<style>` & `<script>` tags
    - LibGuides will come with a number of default css configurations we can't easily remove without breaking searching/subject view things.
# Design Notes
- [Our Figma Project](https://www.figma.com/design/sTxIk3kZhqVAVE7eAGqGH3/SLC?node-id=1-9384&t=Tm2fjONQBzFeh19G-0)
- https://library.rrc.ca/home
- [Wentworth Institute of Technology Libguides](https://library.wit.edu/home)
    - [Their Github Project Page](https://github.com/Adam-Shire-WIT/libguides2-customizations?tab=readme-ov-file)
- [[LibGuides ABC.xlsx]] - From Aviva
- Use case Ideas
    - Booking rooms
    - Mention what you can book on library catalogue page
    - google form as quicker email method w/ formatting
    - custom nav for stats - go to guide, not page within guide.
- Guide Type - How we use them...
    - General Purpose - Website Pages & Clubs
    - Course Guide - Assignments
    - Subject Guide - What Is..?
    - Topic Guide - How To..?
    - Internal Guide - Deprecated Pages & Internal Notes (these are hidden from patrons)
    - Template Guide - Templates (none exist at the moment) (these are hidden from patrons)