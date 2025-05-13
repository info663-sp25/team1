---
title: About
layout: about
permalink: /about.html
# include CollectionBuilder info at bottom
credits: true
# Edit the markdown on in this file to describe your collection
# Look in _includes/feature for options to easily add features to the page
---

{% include feature/jumbotron.html objectid=ph109842 %} 

{% include feature/nav-menu.html sections="About the MAP Project;Process; Project Principles;Functional Requirements;About the Collection" %}

# About the MAP Project
**Objective:** 
  Produce a metadata application profile (MAP) for the assigned collection.   

**Process**:
1. Establish project principles.
2. Form functional requirements.
3. Create a domain model based on the initial functional requirements.
4. Define an element set.
5. Create and implement a metadata entry mechanism with relevant cataloging guidelines.
6. Configure proper crosswalks from chosen elements to Dublin Core and schema.org.
7. Create and deploy a CollectionBuilder website.

## Project Principles
1.  **Accessibility & Usability:**
+ The catalog is being designed for ease of use by art historians and researchers. As a result, the metadata is being structured so that photographs in the collection can be easily searched, browsed, and sorted based on research needs of those with varying levels of research experience or subject familiarity.
+ As a result, any work available online as a result of this project should be made as accessible as possible through the use of Collection Builder features such as “image_alt_text” and “object_transcript.” As a part of this principle, we welcome and appreciate feedback on collected metadata and see formulating access as an ongoing aspect of this project.
2. **Historical Accuracy & Integrity:**
+ Metadata will be based on inscriptions from the backs of photographs, and where possible, these will be verified from scholarly sources researching the archive. Attributions will be true to Bernard Berenson’s classifications; no speculative or ambiguous labels will be used. Works will only be credited to the specific artist. Related works will only be cataloged as they are mentioned by Bernard Berenson or historical scholarship.
3. **Transparency & Documentation:**
+ The source of both the artworks and the photographs will be documented in detail based on metadata on the back of the photographs and Bernard Brenson’s publication, The Venetian Painters of the Renaissance. Images of both the recto and verso sides of the photographs will be made available to researchers. Version control will be implemented for metadata updates, as well as archival descriptions demoting the reasons metadata has been amended. Documentation will be maintained as needed to ensure usability and repeatability of this project.
4. **Community Engagement and Contribution:**
+ Mechanisms will be put in place to allow users to communicate their knowledge on the current locations of the artworks. There will also be a place for users to provide feedback on the catalog. This could be done through a private submission channel on the website to assure that information is adequately assessed and visible to catalogers.
5. **Ethical Representation, Attribution, and Data Ethics:**
+ Metadata sources will be acknowledged and proper attribution will be made for any biases in the historical attributions, such as in the related works field. Any current input from researchers or institutions will be respected in terms of privacy and intellectual property. Rights to photographs will be respected, and photographs will not be shared virtually unless the archive has explicit rights to the image.
6. **Sustainability and Preservation:**
+ The metadata structures will be consistent with the standards for the preservation of digital materials in the long term to ensure accessibility and usability of the information in the future. Priority will be given to the preservation of information relating to the photograph and descriptive metadata and not the preservation of digital files, as fixity checks are often environmentally unsustainable and costly.

## Functional Requirements
Schema Requirements:
| Element      | Search          | Browse  | View  | Sort  |
| ------------- |:-------------:| -----:| -----:| -----:|
| **Title** | X      |    X |    X |    X |
| **Artwork ID** | X      |    - |    X |    - |
| **Artist**     | X | X | X | X |
| **Artwork Size** | -      |    - |    X |    - |
| **Provenance** | X      |    - |    X |    - |
| **Medium** | -      |    - |    X |    - |
| **Bibliographic References** | -     |    - |    X |    - |
| **Subject(s)** | X      |    X |    X |    - |
| **i Tatti ID** | X      |    - |    X |    - |
| **Photographer**      | X      |   X |   X |   X |
| **Filename** | -      |    - |    - |    - |
| **Image Source**      | -      |   - |   X |   - |
| **Print Type**      | -      |   - |   X |   - |


> System Requirements:
>
> + Link filename(s) and identifier(s) to descriptive metadata records
> + Ensure metadata adheres to controlled vocabularies and schema standards (i.e., Dublin Core and VRA Core, Getty Vocabularies, LOC Subject Headings)
> + Support metadata import/export in standardized formats (CSV, XML)
> + Implement version control for metadata updates
> + Enable relationships between works, artists, and collections
> + Allow for hierarchical relationships (e.g., series, sub-series, items)
> + Support external authority files (i.e., Getty ULAN, Library of Congress)


# About the Collection

This collection includes photographs from the Photo Archive of the Berenson Library at Harvard’s Villa I Tatti featuring works of Italian Renaissance art by painters from the Venetian school. The selected photographs come from the “Homeless Paintings of the Italian Renaissance” project—artworks whose locations are currently unknown.

Artworks are represented by photographs which feature stamps and handwritten inscriptions.

The website is built using [CollectionBuilder-CSV](https://github.com/CollectionBuilder/collectionbuilder-csv).

/*Can continue adding here if neded

{% include feature/card.html header="The Astronomer (verso) (Example)" text="Example of the verso of a photograph featuring stamps and inscriptions." objectid="ph109707v" width="25" centered=false%}{% endraw %}
