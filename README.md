# YHS-LibGuide-Customizations
 This a customization project for York House School's Senior Learning Commons LibGuides 2 website.

- `/overrides` contains the actual code affecting the website.
- `/SLC - Archive for Live Server` is an archive of the website from Jan 14, 2025. It is used to provide a *somewhat functional* live server for development. Note that the archive cannot record dynamic content, such as our "All Databases" page.
- `YHS_database_list` .csv & .numbers files are for updating our list of databases

# To Do...
- Styling Ideas
	- Would be nice to move the guide subject list to top of page, for visibility
	- afix nav to top of screen
	- make nav highlight current page https://stackoverflow.com/questions/34491182/make-bootstrap-tab-active-on-the-bases-of-url-link
	- Apply brand colours to site
	- Could use JS script to check subject in subject list, and add specific content to the list page?
- Content Ideas
	- Write a friendly intro in the custom template for 
		- A-Z databases
		- Subject & Subject Landing pages
	- Courses? https://library.rrc.ca/LEARN_modules
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
		- Iconography for common questions
			- Printing Help
			- FAQ
			- Citing
			- Book a Tutor
			- Book a Room
			- Upcoming Events - feature calendar?
		- Feature new library materials - Books, magazines, etc
	- Guide Page
		- internal guide nav menu on left side

# LibGuide Limitations
- We are developing overrides for existing LibGuides conventions, and do not have the entire codebase to host in a live server. To combat this, an archive of the website was made using HTTrack. 
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
- The website depends on several google drive files, as a way to protect PII behind a google login. They are all in [this folder in Kaleb's drive](https://drive.google.com/drive/folders/1udwNokphi7hSrDBAW7WRa8ySkBLZvj1Y)
	- Book Request - Form & Spreadsheet
	- Book Review - Form & Spreadsheet
	- Contact Us - Form & Spreadsheet
	- Database Links/Logins - Multi-slide Presentation
	- Featuring Angela - 1 slide Presentation
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