# YHS-LibGuide-Customizations
 This a customization project for York House School's Senior Learning Commons LibGuides 2 website.

- `/overrides` contains the actual code affecting the website.
- `/SLC - Archive for Live Server` is an archive of the website from Jan 14, 2025. It is used to provide a *somewhat functional* live server for development. Note that the archive cannot record dynamic content, such as our "All Databases" page.
- `YHS_database_list` .csv & .numbers files are for updating our list of databases

# To Do...
- Styling Ideas
	- Fix the broken dropdown menus on individual guides
	- afix nav to top of screen when scrolling
	- make nav highlight current page https://stackoverflow.com/questions/34491182/make-bootstrap-tab-active-on-the-bases-of-url-link
	- Tailwind for static elements (see figma board)
- Content Ideas (Kaleb)
	- Write a friendly intro in the custom template for 
		- A-Z databases
		- Subject & Subject Landing pages
	- add to resources
		- ILL Request
		- snopes
		- internet archive
		- Standard E-Books (well formatted e-books of open source books, and older books with expired copyright) https://standardebooks.org/ebooks?query=frankenstein&sort=newest&view=grid&per-page=12
		- World in data https://ourworldindata.org/
	- Posts to feature new library materials - Books, magazines, etc
- Figma implementation
	- Footer
		- `(#s-lib-footer-login-link > a).href` extract from old footer into custom footer
	- sidebar - mobile visiblity button
	- Home page - Iconography for common questions
		- Printing Help
		- FAQ
		- Citing
		- Book a Tutor
		- Book a Room
		- Upcoming Events - feature calendar?
	- Guide Page
		- internal guide nav menu on left side
		- extract subjects from footer, push to heading: `(#s-lg-guide-header-subjects a).each. "href. &.text"`
	- Search Results

# LibGuide Limitations
- We are developing overrides for existing LibGuides conventions, and do not have the entire codebase to host in a live server. To combat this, an archive of the website was made using HTTrack. 
- Don't have a way to upload custom fonts - need to use [google hosted fonts](https://fonts.google.com/).
- Can upload custom images. They take a day to update when deleted or replaced.
- Can edit individual HTML templates for:
    - Homepage
    - Guides
    - Search Results
    - Subject Page
    - Profile
    - A-Z Guide Browser
- Can edit CSS & JS: Site-wide, or embed in per-page `<style>` & `<script>` tags
- The Site-wide navigation (header.html) cannot autopopulate, and must be manually specified. The required data (links, titles & tags) are not available on every page, and cannot be saved anywhere.
	- It might be possible to fake the API call SpringShare uses to populate the default homepage... but it's more trouble than it's worth.
# Design Notes
- [Our Figma Project](https://www.figma.com/design/sTxIk3kZhqVAVE7eAGqGH3/SLC?node-id=1-9384&t=Tm2fjONQBzFeh19G-0)
- https://library.rrc.ca/home
- [Wentworth Institute of Technology Libguides](https://library.wit.edu/home)
    - [Their Github Project Page](https://github.com/Adam-Shire-WIT/libguides2-customizations?tab=readme-ov-file)
- LibGuides ABC.xlsx - From Aviva
- brooklyn public library case study https://medium.com/design-bootcamp/restructuring-the-brooklyn-public-librarys-information-architecture-c9675a313ff1
- The website depends on several google drive files, as a way to protect PII behind a google login. They are all in [this folder in Kaleb's drive](https://drive.google.com/drive/folders/1udwNokphi7hSrDBAW7WRa8ySkBLZvj1Y)
	- Book Request - Form & Spreadsheet
	- Book Review - Form & Spreadsheet
	- Contact Us - Form & Spreadsheet
	- Database Links/Logins - Multi-slide Presentation
	- Featuring Student - Multiple 1 slide Presentations
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