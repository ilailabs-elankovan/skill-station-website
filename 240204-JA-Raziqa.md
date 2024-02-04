## Skill Station Website Asset Preparation

**Instructions to the Designer**

**I. Asset Preparation**

[Figma file URL](https://www.figma.com/file/tXK6HPmBObsQvHYSfRTDpa/SkillStationWeb?type=design&node-id=0%3A1&mode=design&t=GpspfuR201W3XSUz-1)

• Export the logo and all the images form the figma file. \
• Ensure the logo is in the sandard size 24x24 or 48x48 and export as SVG. \
• Images of particular section or set must be of same size. Ensure to resize the images by re-working them in a seperate artboard. \
• For gif in the *Hero Section* download them from [this page](https://ilailabs.github.io/profile-elankovanmg/images/gallery.md.html) and directly paste in inside the `assets/images` folder. \
• Add images to the existing folder `assets/images/<file_name.png> with proper naming convention. User only *snake case*, example *skill_station_logo.png* \

**II. JSON File Preparation**

Fill the below Json file with appropriate URLs and Contents form the Design. 

Use this prefix `https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/<file-path>`

**1. Common Page Icons**

Collect all the common page icons here. 

```json
var assetUrls = {
  "logo": "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/logo.svg",
  "whatsapp_icon":"https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/whatsapp_icon.svg",
  "internship_icon":"https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/internship_icon.svg",
  "career_guidance":"",
  "workshops_icon":"",
  "courses_icon":"",
  "fb_icon":"",
  "yt_icon":"",
  "phone_icon":""  
};
```

*NOTE:* You can use ChatGPT with this prompt given below to complete the given task easily:

```
Complete the Json file given below. 

{
  "logo": "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/logo.svg",
  "whatsapp_icon":"https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/whatsapp_icon.svg",
  "internship_icon":"https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/internship_icon.svg",
  "career_guidance":"",
  "workshops_icon":"",
  "courses_icon":"",
  "fb_icon":"",
  "yt_icon":"",
  "phone_icon":""  
}

Use the key name as reference to generate the corresponding key value. 
Example if key name is 'logo' then generate a key value such that 'logo.svg'. 
To give you an another example if key name is 'whatsapp_icon' then generate a corressponding key value as 'whatsapp_icon.svg". 
One you generated the key value pair add a prefix "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/" to the string "logo.svg" in the key value pair. 
Complete the same for all the key value pair.
```

**2. Hero Section**

```json
var heroSection = [
  "section_title": "Empowering Minds/nTransforming Lives/nTogether We Educate",
  "button1_title": "Volunteer with us",
  "button1_text": "For students, mentors and educators",
  "button1_url": "https://wa.me/919940275422" // todo: Update the skill sation number here; Later we can update the gForm Link here.
  "bg_sliders": [
      "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/bg_image0.gif",
      "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/bg_image1.gif",      ]
  ];
```

**3. What We Do Section**

```json
var whatWeDoSection = [
  {
    "card_icon1": "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/bg_image0.gif",
    "card_title": "Internships & Placements",
    "card_text": "Skill Station has collabrated with various startups and organisations for their hiring needs. We ensure you land up a internship position right after the course completion. Depending on the candidates performance this can be a paid or non-paid internship"
  },
  {
    "card_icon1": "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/bg_image0.gif",// todo: edit this; 
    "card_title": "Internships & Placements", // todo: edit this; 
    "card_text": "Skill Station has collabrated with various startups and organisations for their hiring needs. We ensure you land up a internship position right after the course completion. Depending on the candidates performance this can be a paid or non-paid internship" // todo: Edit this
  },
  {}, // todo: edit this
  {} // tood: edit this
];
```

**4. Who We Are Section**

```json
var whoWeAreSection = {
  "section_text": "Skill Station is a non-profit ... young minds." // todo: complete this.
  "read_more_url": "" // todo: we must include the linkedin page url here.
  "section_images": [
    "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/about_image0.png",
    "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/about_image0.gif"
  ],
  },
```

**5. Courses We Offer**

```json
var coursesWeOfferSection = [
  {
    "card_url":"https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/course_image0.png",
    "card_title":"Full Stack Web Application Development(MERN)"
    "card_chip_text":["Fundamentals of Javascript", "Introduction to Web Application Development with ReactJs", "Introduction to Server Side App Development with NodeJs"],
    "card_chip_footer_text":["Beginner", "Professional", "3 Months"],
    "card_button1_url": "" // todo: add course broucher gDrive link here; This is for View More,
    "card_button2_url": "" // todo: we shold add the gForm link here; the will be udpated once I creat it;
  },
  {}, // todo: Edit the same for card 2 flutter course
  {} // todo: Edit the same for card 3 Html Css course; refer the course broucher for details.
  ];
```

**6. Students Feedback Section**

```json
var studentsFeedback = [
  {
    "card_text":"Skill Station Academy Provided me an exceptions ...",
    "card_avatar_url": "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/student_avatar0.png"
    "student_name": "Varun",
    "student_title": "UI/UX Designer"
  },
  {}, // todo
  {}, // todo
  {} // todo
  ];
```

**7. Workshop Section**

```json
var ourUpcommingWorkshops = [
  "Devlops Course Comming Soon",
  "AI-Workshop will be updated shortly"
]
```

**8. Our Hiring Partners Section**

```json
var ourHiringPartners = [
  "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/partners_image0.png",
  "https://raw.githubusercontent.com/ilailabs-elankovan/skill-station-website/main/assets/images/partners_image1.png"
];
```

**9. Footer Urls**

```json
var footerUrls = {
  "about_skill_station":"#about_skill_station",
  "professional_courses":"#professional_courses",
  "events": "#events_workshops",
  "workshops": "#events_workshops",
  "internships": "#internships_placements",
  "placements": "#internships_placements",
  "contact_us":"https://wa.me/91...", //todo: update number here;
  "feedback": "" , // todo: lets create a course feedback form here;
  "linkedin_page": "", // todo: update only the linked in page as of now; remove the fb, yt, icons in figma;
  "email": "mailto:info@skillstation.org" // add this button in the footer section; 
  "whatsapp":"https://wa.me/91...", // update here; 
  "phone": "", // levae this empty for now; 
};
```


