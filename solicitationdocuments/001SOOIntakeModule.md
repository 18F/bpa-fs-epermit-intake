# 18F Agile Blanket Purchase Agreement

# Request for Quotation

# Statement of Objective

# 1.0 BACKGROUND

## Forest Service Permitting

The U.S. Forest Service is engaged in an ongoing effort to modernize and simplify their permitting processes. One facet of this effort is “ePermitting”, or making the applications for many Forest Service permits available online.

This application is for a public front-end intake module for use by non-commercial groups, temporary outfitter, and guide permits. This application will collect the application information for such special use permits then present it to the Forest Service’s special use administrators thereby allowing them to “accept” an application and pre-populate an entry in the Forest Service’s Special Uses Data System (SUDS) via a RESTful Application Protocol Interface (API).

This application must be centered on the needs of its **end users**, as follows:

-   Outfitters and guides who apply for permits;

-   Schools and higher education institutions leading trips in National Forests;

-   Non-profit clubs and organizations (such as the Boy Scouts, YMCA, mountaineering groups); and,

-   Special use administrators (the people who manage the process of distributing permits at the forest level).

This application will be used by a single pilot forest initially, the Mt. Baker-Snoqualmie National Forest, but should be built so as to scale across multiple Forests, districts, and permit administrators. Additional end users and permittees may be contemplated at a later date. In order to assist comprehension of this effort, 18F has created a prototype at [*https://github.com/18F/forest-service-prototype*](https://github.com/18F/forest-service-prototype)

## Prototype

If respondents chose to use the prototype, they will need to modify it to support all the user stories listed in the performance objectives provided in Section 2.

Respondents who use the prototype may also need to remove some functionality the prototype no longer needs (and is not covered by the user stories listed in the performance objectives). For example, the current prototype can generate a printable permit, while the finished application should not have that ability.

## User stories supported by the prototype

The prototype currently supports a subset of the user stories from this RFQ’s objectives as follows.

### From the “submitting a non-commercial group use permit application” section:

-   As a non-commercial group use applicant, I want to submit the information the Forest Service needs to issue my permit (described in form [FS-2700-3b]([*http://www.fs.fed.us/specialuses/documents/fs-2700-3b.rtf*](http://www.fs.fed.us/specialuses/documents/fs-2700-3b.rtf)) )

### From the “submitting an application” section:

-   As an applicant, I want to have the opportunity to correct minor errors before submitting my application.

-   As an applicant, I want confirmation my application was successfully submitted and a description of what will happen from here.

-   As an applicant, I receive an estimate as to when my application will be approved (not just when I’ll receive a response) when I submit my permit application.

-   As an applicant, I would like a way to cancel my application after I submit it.

-   As an applicant, I would like to be able to check back on the application after I submit it.

# 2.0 PERFORMANCE OBJECTIVES

The following user needs shall be met in order to fulfill the objectives for performance of this task order, and may be refined by later sprints to continuously meet user needs. In agreement with the product owner, user stories can be modified, added, retracted or reprioritized.

## User stories for Front-end layer

18F has created a prototype available at: [*https://github.com/18F/forest-service-prototype*](https://github.com/18F/forest-service-prototype)

Offerors may make use of this prototype at their discretion, use another JavaScript framework, or Ruby on Rails.

Some of the user stories described in this section have already been met by the current prototype. If respondents choose to use the prototype, they will need to modify it to support all the stories listed here. (The user stories currently supported by the prototype are listed in the “Current Prototype Functionality” addendum.) Respondents who use the prototype may also need to remove some functionality it no longer needs (and are not covered by the following user stories).

### Choosing a permit

-   As an applicant, I would like to have the ability to select the specific National Forest to submit an application to.

-   As an applicant, I would like to know whether or not the activity I am requesting requires a permit.

-   As an applicant whose activity requires a permit, I would like to know whether or not the activity I am requesting requires a permit fee and how much that fee will likely be for my proposed activity.

-   [As an applicant, I want to choose](https://github.com/18F/forest-service-prototype/issues/4) what type of permit application to complete based on a set of questions around my interest in doing an activity on the forest and a brief description of each permit.

-   As an applicant, I want instructions about where to go if I don’t see the permit I need in this list.

### Submitting a non-commercial group use permit application

-   As a non-commercial group use applicant, I want to submit the information the Forest Service needs to issue my permit (described in form [FS-2700-3b]([*http://www.fs.fed.us/specialuses/documents/fs-2700-3b.rtf*](http://www.fs.fed.us/specialuses/documents/fs-2700-3b.rtf)) )

### Submitting a temporary outfitter / guiding permit application

-   As an outfitter / guide applicant, I want to be able to learn about the basic restrictions of a temporary (3 year) permit.

-   As a non-commercial group use applicant, I want to understand the process for submitting an application (what steps I will take now, what will happen after that, etc.). In particular, I want to know what documents I will be required to compile and attach.

-   As an outfitter / guide applicant, I want to choose what activity I want to lead and view a list of places where I can receive permits to do them.

-   As an outfitter / guide applicant, I want to understand the restrictions and due dates for permits on each place I could do each activity.

-   As an outfitter / guide applicant, I want to be able to select an activity that isn’t in the list, describe it briefly and select whether it’s land or water-based.

-   As an outfitter / guide applicant, I want to submit the information the Forest Service needs to issue my permit (described in form [FS-2700-3f](http://www.fs.usda.gov/Internet/FSE_DOCUMENTS/stelprdb5251858.docx))

-   As an outfitter / guide applicant, I can attach necessary documentation, including a required operating plan and insurance certificate.

-   As an outfitter / guide applicant, I would like an estimate of the initial and final fee I will have to pay for my permit (as well as an explanation of when I will pay).

### Submitting applications

-   As an applicant, I want to have the opportunity to correct minor errors before submitting my application.

-   As an applicant, I want confirmation my application was successfully submitted and a description of what will happen from here.

-   As an applicant, I receive an estimate as to when my application will be approved (not just when I’ll receive a response) when I submit my permit application.

-   As an applicant, I receive the name, email address and phone number of the [Forest Service special uses administrator](https://github.com/18F/forest-service-prototype/issues/2) receiving my application.

-   As an applicant, I would like a way to cancel my application after I submit it.

-   As an applicant, I would like to be able to check back on the application after I

submit it.

### Accepting an application and send a request to the Special Uses Data System API to store the permit information.

*Currently, when Forest Service special uses administrators receive permit applications, they review them and manually enter them into the Special Uses Data System (SUDS). From SUDS, they generate a final permit document and invoice (if applicable). This “intake module” will allow special use administrators to review permit applications submitted online, choose which applications to “accept”, and upon acceptance send the permit information to the SUDS API.*

-   [As a Forest Service special uses administrator, I want to see a list and the content of applications](https://github.com/18F/forest-service-prototype/issues/2) I have received to my Forest that are pending.

-   As a Forest Service special uses administrator, I would like to be able to accept an application and send a request to the API to enter that information into SUDS.

-   As a Forest Service special uses administrator, when I accept an application, if a similar name (or organization name) appears in the SUDS contact database (queryable via the SUDS API), I will be able to associate the application with an existing contact name.

-   [As a Forest Service special uses administrator, I](https://github.com/18F/forest-service-prototype/issues/2) would like to receive an email when a new application is submitted to my Forest.

-   As a Forest Service special uses administrator, I would like to receive an email if an application has been cancelled by the application submitter.

-   As a Forest Service special uses administrator, I would like to be able to close a not yet approved application, but only after a reminder to email the participant and explanation of why the application is being deleted.

-   As a Forest Service special uses administrator, I would like to be able to access approved and closed applications.

-   As a Forest Service special uses administrator, when the application is accepted, explaining what will happen next. *Permits are not “approved” until a later stage; this intake module would only handle processing applications from receipt to “acceptance,” while SUDS handles the rest of the process.*

### Settings

-   As a Forest Service special uses administrator, I would like to be able to customize the contents of the emails applicants receive (in an online administrative interface) when they submit applications and when they are approved.

-   As a Forest Service special uses administrator, I can configure the estimated fees, due dates, response and approval time estimates the system displays for my Forest.

## Application Constraints:

-   Hosted in a linux environment, or possibly using Cloud.gov

-   The Contractor may use the existing Forest Service prototype at [*https://github.com/18F/forest-service-prototype*](https://github.com/18F/forest-service-prototype), or may use another JavaScript framework, or Ruby on Rails.

-   The front-end application must connect to an API that will use future iterations of the [*linked data-schema.*](https://github.com/18F/forest-service-permit-api-schemas/tree/master/special-use)

-   Personal Identity Information (PII) shall be secure and kept through encryption from exposure to unauthorized users from uploaded documents.

-   Authentication for public users, possibly using Login.gov is available by the period of performance.

-   Authentication with USDA e-Auth for FS employees.

## Additional requirements:

-   At sprint-wise intervals, the vendor will open issues that came as the result of usability testing by end-users.

-   Contractor shall use [*US Web Design Standards.*](https://playbook.cio.gov/designstandards/)

-   All software code delivered under this order shall comply with the [*18F open source policy*](http://https/github.com/18F/open-source-policy/) in effect as of the date of award.

-   All software code delivered under this order shall comply with the [*18F Accessibility Guidelines*](https://pages.18f.gov/accessibility/) in effect as of the date of award.

-   As part of this being purchased off of the Agile Blanket Purchase Agreement (aBPA), work will be conducted in one or two-week sprints and reviewed at the end of each sprint for acceptability per the Quality Assurance Surveillance Plan (QASP).

# 3.0 SCOPE

This application is an intake module for all special uses permitting. To satisfy the needs of non-commercial groups, temporary outfitter, and guide permits, the following deliverables must be provided by the conclusion of performance.

#### 3.1 List of Deliverables

**| DELIVERABLES | DUE DATES | CONTENT DESCRIPTION |**
|:----------:|:-------------:|:------:|
| Code Repository of Product | Ongoing with every applicable sprint | Version-controlled Open Source repository of code that comprises product that will remain in the public domain |

| Issues in repository from usability testing | Ongoing with applicable sprint | Usability or other issues discovered via usability testing and documented in the project’s source control system |
| Design Deliverables | Ongoing with every applicable sprint | Mock ups and/or design files if applicable, or design changes reflected in the Development Product |

| Issues from user testing | Ongoing with applicable sprint | Issues raised by user testing |
| Development Product | Ongoing with applicable sprint | In-progress development product, accessible on the web via staging server / development server |

| Transition plan | Per direction of COR | Provided in QASP |

# 4.0 PROPOSED PERSONNEL

## 4.1 Desired Skills and Knowledge

Offerors shall provide qualified personnel commensurate with this task's performance work statement, in terms of necessary skills at the requisite level of knowledge and experience.

Proposed personnel shall have a strong technical experience base in the following:

-   Technology stack as delineated in Section 2.0.

-   Building front-end applications that process data from and send data to a RESTful API

-   Using human centered design methods to build and test form-driven, web-based applications. Human-centered design practices include:

    -   Research, such as (but not limited to) contextual inquiry, stakeholder interviews, and usability testing

    -   User experience design

    -   Front end development

    -   Sketching, wireframing, and/or prototyping

    -   Visual design

    -   Content design

-   “Mobile first” approaches, performance budgeting, and progressive enhancement

-   Building and testing public facing sites and tools

-   Open source software development

-   Cloud deployment

-   Open-source login/authentication services

-   Low-bandwidth environments

-   Managing and securing PII

-   Agile and Scrum methodologies

## 4.2 Key Personnel

**For this task the following Key Personnel are necessary (as detailed at [https://pages.18f.gov/agile-labor-categories/](https://pages.18f.gov/agile-labor-categories/)): **

-   **Product Manager**

-   **Interaction Designer / User Researcher / Usability Tester**

-   **Offerors must choose only 1 of any of these 3 labor categories as the third Key Personnel position Technical Architect / Backend Developer / Frontend Developer**

# 5.0 INSTRUCTIONS

## 5.1 Milestones

Quotes must be valid for at least 45 calendar days after quotation response date. Information provided in the quotation shall be concise, specific, and complete.

Offeror(s) shall direct all written or verbal communications during this process to the Contracting Specialist. Communications with other officials may compromise the competitiveness of this acquisition and result in removal of the offeror from award consideration or cancellation of this requirement.

Offerors shall submit a signed Potential Organizational Conflict of Interest Statement (COI). If the offeror does have any potential organizational conflicts of interest, they shall provide a statement describing the potential or actual COI with their quote. Information contained must be accurate and complete to allow for a CO reasonable and meaningful consideration of any potential or actual COI determination.

COI responses must be provided in the appropriate field of the provided Google Form order to be considered for award.

**The Government intends to accomplish the quote and evaluation process in 2 distinct phases. **

The following milestones are provided for this solicitation.

**| No. | DUE DATES | ACQUISITION EVENT |**
|----------|:-------------:|------:|
| 1 | February 15, 2017 | Solicitation Released |
| 2 | February 17, 2017 by 3:00PM EST | Questions about Solicitation Due |
| 3 | February 28, 2017 by 1:00PM EST | Written Quote Submissions Due |

Questions or comments regarding this RFQ shall be submitted as issues within the GitHub repository at [*https://github.com/18F/bpa-fs-epermit-intake*](https://github.com/18F/bpa-fs-epermit-intake) no later than **February 17, 2017 at 3:00 pm EST**, to allow the Government sufficient time to respond. All questions and comments will be publicly available. Please subscribe to the repository if your firm would like updates about changes and comments. Questions or comments received after the required deadline will not be answered. Any changes to this RFQ or attachments will be posted as an amendment on GSA eBuy.

## 5.2 Phase 1 - Quote Submission

## 5.2.1 Technical Quote

To decrease the burden on potential Offerors, a Google Form has been provided for the written technical quote portion of submissions. Only one submission will be evaluated (no alternate proposals will be allowed). **All offers must be received no later than February 28, 2017 at 1:00PM EST.**

**Written technical quotes will only be accepted via the provided Google Form.**

If potential offerors do not submit this completed Google Form they will be deemed non-compliant and excluded from consideration for award. No other format of a written technical quote will be deemed acceptable by the Government.

The Google Form is available here: [[*https://goo.gl/forms/j29QwBoRNA5cMzPK2*](https://goo.gl/forms/j29QwBoRNA5cMzPK2)]

All of the information below is provided via the fields of the Google Form above.

**For the Technical Quote, provide:**

-   **Technical Understanding and Approach** This will be Factor 1 for the purposes of technical evaluation. Offerors shall provide their understanding of the performance objectives for the requirements as described in Section 2.

    Offerors shall also describe their staffing plan based on their technical understanding and approach for the requirements with their estimated level of effort to complete. The estimated level of effort shall include a breakdown of labor categories, including the title, number of personnel, and hours.

    All proposed skill levels/labor categories shall be consistent with the Offeror’s aBPA award. All price related information shall only be provided separately and apart from the written technical quote.

-   **Key personnel.** This will be Factor 2 for the purposes of technical evaluation. The offeror shall provide a list of key personnel by name, title, contact information, proposed duties and roles, and resumes for each proposed key personnel in accordance with Section 4.2 of this solicitation.

    Resumes should include a brief description of the experience and capability for all key personnel proposed for the Offeror’s project team. Resumes should also address the individual’s technical background, education, work experience, and accomplishments related to the activities described in this solicitation. For the technical architect, back-end web developer or front-end web developer position, please include the key personnel’s GitHub repository as part of your resume.

    The quote of any key personnel not currently employed by the offeror or teaming partners shall be accompanied by letters of intent signed by proposed key personnel in accordance with Section 4.2 of this solicitation.

-   Resumes and letters of intent are not included as part of any page limitation for the quote . **Resumes cannot exceed 1 page in length.**

-   **Similar Experience - Code Repository Submission**

    The code repository will be Factor 3 - Similar Experience for the purposes of technical evaluation.

    All potential offerors must submit two publicly available code repositories as a signal of intent to bid. Only those Agile BPA awardees who submit two a publicly available code repositories in the same language proposed for this requirement will be considered and advance to the Phase 2. The code repository provided must be in the same programming language as any potential offeror would choose to use for the intake module itself.

    Any potential offeror who fails to submit two code repositories in the same language as proposed for this requirement will be deemed non-responsive and shall not move onto to any later stages or be considered for award.

    The cited similar experience will be the two live code repositories submitted and will not require any further documentation.
    Code repositories must be in the same runtime language as proposed for this effort and similar in similar size, scope, and complexity.

    Code repositories submitted must have been for projects completed within the past three (3) calendar years, with staffing profiles of approximately four (4) to five (5) Full Time Equivalent (FTE) personnel in periods of performance lasting no more than six (6) calendar months.

-   The projects must have been delivered by either a) the Offeror itself or, alternatively, b) a teaming partner that is proposed in response to this solicitation, or, alternatively, c) any key personnel that is being proposed in response to this solicitation. Please identify how the offeror’s team was involved in the development. Offerors that include similar experience of the same key personnel who directly participated in the cited similar experience will be ranked higher than those who propose projects that did not involve their key personnel.

    Links to the Git repository (either credentialed or public) that includes the source code that was developed and accepted for the project must be provided in the appropriate field of the provided Google Form order to be considered for award.

Written technical quotes that fail to include any of the items identified above will not be considered for award. Inclusion of caveats, assumptions, or exceptions to the requirement of any kind, in any part of the submission, will result in the Offeror no longer being considered for award.

If potential Offerors intend to use any Contractor Teaming Arrangements CTAs/Subcontractor arrangements, then they must provide a description of it that includes company names, personnel, and the parts of performance to be provided. Because CTAs and subcontractor arrangement are not the same, Offerors shall clearly identify if they are proposing a CTA or subcontractor arrangement. If the offeror is not proposing any CTAs/subcontractor arrangements, then they are not required to do anything to indicate that they are not doing so.

###5.2.2 Written Price Quote

The Government hereby seeks further price reductions and Most Favored Customer (MFC) pricing for all proposed services. Offerors are advised to provide your best discounted rates.

Offerors shall submit a separate price quotation via the provided worksheet template in the eBuy system. **The price quotation must be received no later than February 28, 2017 at 1:00PM EST.**

All proposed labor rates shall be consistent with your the terms, conditions, and rates of your aBPA. Proposed labor rates must be fully burdened, inclusive of profit, fringe benefits, salary, indirect rates, and the GSA Contract Access Fee (CAF).

## 5.3 Phase 2 - Oral Presentation

Oral presentations will only be scheduled with potential offerors who have successfully advanced through phase 1.

### Oral Presentations Agenda

**| No. | AGENDA ITEM | MAXIMUM TIME |**
|----------|:-------------:|------:|
| 0 | Government Provides Oral Questions to Offeror (e-mail) | Approximately 60 minutes Prior to Oral Presentation minutes |

| 1 | Introductions | Approximately 5 minutes |
| 2 | Technical Session | 25 minutes |
| 3 | Break For Offeror & Government Questions | 5 minutes |

| 4 | Follow Up Session (if needed) | 15 minutes |

### Rules

No aspect of these oral presentations constitutes a procedure in FAR Part 15, such as discussions or negotiations. Therefore, the Government is not obligated to and will not determine a competitive range, conduct discussions, and request quote revisions.

The oral presentation consists of an initial question and answer session on technical factors, and, if necessary, a follow-up question and answer session. The entire oral presentation will be conducted remotely via video and audio.

Offerors shall not make use of, provide, or present slides, graphs, charts or any other written presentation materials nor will the Government accept or receive Offeror handouts.

### Content
The Technical Session will consist of the answering the Government’s core questions related to the technical factors identified in this solicitation.

While the technical factors are identified in the RFQ, the core questions are
not. All Offerors will be asked the same core questions related to the technical factors.

This part of the oral presentations will not exceed 25 minutes. The Contracting Officer will strictly enforce this time limit on all presentations.
Note that each Offeror will be provided the Technical Session questions, via e-mail, approximately 60 minutes prior to their Oral Presentation. The goal of these presentations is to assess the technical abilities of the proposed Key Personnel and further elaborate on their proposed technical approach to accomplish the objectives of this task.

The Government may take notes during the presentation at its discretion and exclusive right and property, and may use such notes in the evaluation. No copies will be provided to the Offeror.

### Follow Ups (only if necessary)
The Government will allocate 15 minutes for follow-up questions following the Offeror’s answers to the core questions on technical factors. This is purely to ensure the Government has understood each Offeror’s responses provided in the Technical Session.

If necessary, the Government may ask followup questions during this time on any answers presented by the Offeror that the Government feels is unclear or needs elaboration to comprehend. The Government’s questions may differ among the Offerors based on what needs elaboration.

If the Government has no follow-up questions with a particular Offeror, then this session won’t occur. The answers given in this session are considered part of the Offeror’s Technical Session, as any question posed is not new but merely clarifying an Offeror’s response.

### Presentation Location
Oral Presentations will be conducted by video chat, though audio may be substituted as needed. The Government will coordinate and set up the meeting space accordingly (providing dial in or links using a tool such as Zoom).

### Presentation Date and Time
The Government will schedule the date and time of the oral presentations with each Offeror after the solicitation closing date and receipt of Offeror quote submissions. The Government reserves the right to reschedule any Offeror’s orals date at the discretion of the contracting officer.

### Presentation Participants
**If proposed Key Personnel do not participate then offerors will be deemed non-compliant and excluded from further consideration.**

Offerors may include as many participants as it feels is necessary. Offerors are advised Government will ask technical questions during the oral presentations primarily regarding actual performance, so non-technical personnel may be of limited purpose.

All proposed Key Personnel currently employed by the Offeror or its teaming partners shall attend the session - the Government is most interested in hearing from staff that will have a direct role in performing on the task.

After the presentations, vendors shall provide an email to confirm attendance with names of participants to the meeting organizers.

# 6.0 EVALUATION

## 6.1 Technical Evaluation Factors

The Government shall evaluate the requirements for an Offeror’s performance or capability acceptability based on the following non-price technical factors which are of equal importance to each other.

The Government will evaluate each submission against the requirements of this solicitation and in accordance with the evaluation factors provided below to determine each Offeror’s demonstrated ability to perform. These factors are of equal importance:

-   Factor 1 - Technical Understanding and Approach

-   Factor 2 - Key Personnel

-   Factor 3 - Similar Experience

## 6.2 Price Evaluation Factors

Each Offeror’s price quotation will be evaluated separately from the technical quotation. The Government will evaluate the Offeror’s proposed price to ensure that the offered price is fair, reasonable, and realistic. Pricing shall reflect reasonableness, consistency with industry standards, and be in compliance with rates and terms and conditions of the aBPA.

## 6.3 Evaluation Process

The Government intends to utilize a two phased quote and staggered evaluation process for this procurement. Of the total potential offerors on the aBPA, only those who satisfy Phase 1 will be evaluated for purposes of award.

### Phased Compliance Check. The Government will review all offers at each phase to ensure compliance with the instructions and requirements set forth in the solicitation. Offerors that are not compliant with the solicitation will not be considered in the next phase.

### Quote Evaluation. Review of written Technical quote and Oral Presentations. The Offeror’s written technical quote and responses to questions asked during the Oral Presentations will be evaluated based on an assessment by the Government technical evaluation team of their strengths, weaknesses, and risks associated with the technical factors described above.

Based upon the Government’s evaluation of each quote’s technical strengths, weaknesses, and risks, the Government will provide a narrative, ordinal ranking of each quote received in terms of the highest to lowest ranked technical quotes.

Following the ranking of technical quotes, price will be introduced and a best value decision will be made in accordance with Section 7 below. The Government will provide a brief explanation in accordance with FAR 8.405-2(d) to unsuccessful offerors upon timely request.

# 7.0 BASIS for AWARD

The final award for this requirement will be based on best-value principles. Accordingly, award will be made to the responsible and technically acceptable Offerors whose quote provides the greatest overall value to the Government, price and other factors considered.

This best-value determination will be accomplished by comparing the value of the differences in the technical factors for competing offers under consideration in the technical evaluation, based on their strengths, weaknesses, and risks, with differences in their price to the Government.

In making this comparison, the Government is more concerned with obtaining superior technical and management capabilities than with making awards at the lowest overall price to the Government. However, the Government will not make awards at a significantly higher overall price to achieve slightly superior technical value. Offerors are advised that the technical evaluation factors combined are significantly more important than price.

# 8.0 AWARDED TASK

This task order is a Firm-Fixed Price type award with a base period of three months and one three-month option period.

The following Points of Contact (POC) are applicable to this order:

Contracting Officer: Name, Phone, Email

Contracting Officer Representative (COR): Name, Phone, Email

Alternative Contracting Officer Representative, if necessary (ACOR): Name, Email

Product Owner: [To Be Determined]

Other pertinent information related to Incorporated Clauses, Invoicing, 18F’s Transparency Policy, Data Rights, Section 508 Compliance, and other incorporated terms and conditions from the contractor’s aBPA are provided in the QASP.

# 9.0 CONTRACT CLAUSES INCORPORATED BY REFERENCE

FAR 52.227-17 Rights in Data -- Special Works (DEC 2007)

FAR 52.217-5 Evaluation of Options (JUL 1990)

# 10. CONTRACT CLAUSES INCORPORATED IN FULL TEXT

### FAR 52.252-1 -- SOLICITATION PROVISIONS INCORPORATED BY REFERENCE (FEB 1998)

This solicitation incorporates one or more solicitation provisions by reference, with the same force and effect as if they were given in full text. Upon request, the Contracting Officer will make their full text available. The offeror is cautioned that the listed provisions may include blocks that must be completed by the offeror and submitted with its quotation or offer. In lieu of submitting the full text of those provisions, the offeror may identify the provision by paragraph identifier and provide the appropriate information with its quotation or offer. Also, the full text of a solicitation provision may be accessed electronically at this/these address(es): ([*http://farsite.hill.af.mil/vffara.htm*](http://farsite.hill.af.mil/vffara.htm))

(End of Provision)

### FAR 52.252-2 -- CLAUSES INCORPORATED BY REFERENCE (FEB 1998)

This contract incorporates one or more clauses by reference, with the same force and effect as if they were given in full text. Upon request, the Contracting Officer will make their full text available. Also, the full text of a clause may be accessed electronically at this/these address(es): ([*http://farsite.hill.af.mil/vffara.htm*](http://farsite.hill.af.mil/vffara.htm))

(End of clause)

### FAR 52.203-98 -- PROHIBITION ON CONTRACTING WITH ENTITIES THAT REQUIRE CERTAIN INTERNAL CONFIDENTIALITY AGREEMENTS-REPRESENTATION (DEVIATION 2015-02) (APR 2015)

(a) In accordance with section 743 of Division E, Title VII, of the Consolidated and Further Continuing Resolution Appropriations Act, 2015 (Pub. L. 113-235), Government agencies are not permitted to use funds appropriated (or otherwise made available) under that or any other Act for contracts with an entity that requires employees or subcontractors of such entity seeking to report fraud, waste, or abuse to sign internal confidentiality agreements or statements prohibiting or otherwise restricting such employees or subcontractors from lawfully reporting such waste, fraud, or abuse to a designated investigative or law enforcement representative of a Federal department or agency authorized to receive such information.

(b) The prohibition in paragraph (a) of this provision does not contravene requirements applicable to Standard Form 312, Form 4414, or any other form issued by a Federal department or agency governing the nondisclosure of classified information.

(c) Representation. By submission of its offer, the offeror represents that it does not require employees or subcontractors of such entity seeking to report fraud, waste, or abuse to sign internal confidentiality agreements or statements prohibiting or otherwise restricting such employees or subcontractors from lawfully reporting such waste, fraud, or abuse to a designated investigative or law enforcement representative of a Federal department or agency authorized to receive such information.

(End of provision)

### FAR 52.203-99 -- PROHIBITION ON CONTRACTING WITH ENTITIES THAT REQUIRE CERTAIN INTERNAL CONFIDENTIALITY AGREEMENTS (DEVIATION 2015-02) (APR 2015)

(a) The Contractor shall not require employees or subcontractors seeking to report fraud, waste, or abuse to sign or comply with internal confidentiality agreements or statements prohibiting or otherwise restricting such employees or subcontractors from lawfully reporting such waste, fraud, or abuse to a designated investigative or law enforcement representative of a Federal department or agency authorized to receive such information.

(b) The contractor shall notify employees that the prohibitions and restrictions of any internal confidentiality agreements covered by this provision are no longer in effect.

(c) The prohibition in paragraph (a) of this clause does not contravene requirements applicable to Standard Form 312, Form 4414, or any other form issued by a Federal department or agency governing the nondisclosure of classified information.

(1) In accordance with section 743 of Division E, Title VII, of the Consolidated and Further Continuing Resolution Appropriations Act, 2015 (Pub. L. 113-235), use of funds appropriated (or otherwise made available) under that or any other Act may be prohibited, if the Government determines that the Contractor is not in compliance with the provisions of this clause.

(2) The Government may seek any available remedies in the event the recipient fails to comply with the provisions of this clause.

(End of clause)

### FAR 52.217-8 -- OPTION TO EXTEND SERVICES (NOV 1999)

The Government may require continued performance of any services within the limits and at the rates specified in the contract. These rates may be adjusted only as a result of revisions to prevailing labor rates provided by the Secretary of Labor. The option provision may be exercised more than once, but the total extension of performance hereunder shall not exceed 6 months. The Contracting Officer may exercise the option by written notice to the Contractor within 10 calendar days before the contract expires.

(End of clause)

FAR 52.2147-9 -- OPTION TO EXTEND THE TERM OF THE CONTRACT (MAR 2000)

#### (a) The Government may extend the term of this contract by written notice to the Contractor within 5 days provided that the Government gives the Contractor a preliminary written notice of its intent to extend at least 15 days before the contract expires. The preliminary notice does not commit the Government to an extension.

#### (b) If the Government exercises this option, the extended contract shall be considered to include this option clause.

#### (c) The total duration of this contract, including the exercise of any options under this clause, shall not exceed 18 months.

#### (End of clause)

GSAR 552.217-71 – NOTICE REGARDING OPTION(S) (NOV 1992)

GSA has included an option to *extend the term of this contract* in order to demonstrate the value it places on quality performance by providing a mechanism for continuing a contractual relationship with a successful Offeror that performs at a level which meets or exceeds GSA’s quality performance expectations as communicated to the Contractor, in writing, by the Contracting Officer or designated representative. When deciding whether to exercise the option, the Contracting Officer will consider the quality of the Contractor’s past performance under this contract in accordance with 48 CFR 517.207.

#### (End of provision)

## ATTACHMENTS TO THIS SOLICITATION

1.  Pricing Template

2.  Quality Assurance Surveillance Plan (QASP) including Task Administration (Invoicing, etc.)

3.  Non Disclosure Agreement

4.  SF1449
