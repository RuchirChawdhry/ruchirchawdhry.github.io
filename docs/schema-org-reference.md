# Schema.org JSON-LD Reference

Selected structured-data vocabulary for the portfolio, open-source software projects and their documentation websites. This is a reference and agreed scope for future centralized generation, not a statement that these schemas are already implemented.

See the [Schema.org vocabulary](https://schema.org/docs/full.html) for definitions and permitted properties.

## Selected schema types

### Website and navigation

| Schema type | Purpose |
| --- | --- |
| `WebSite` | Identify a website |
| `WebPage` | Describe an individual webpage |
| `BreadcrumbList` | Navigation hierarchy |
| `CollectionPage` | Project and documentation directories |
| `ItemList` | Lists of projects and resources |
| `ListItem` | Individual list entries |
| `AboutPage` | Project or developer information |
| `ProfilePage` | Developer profile |
| `ContactPage` | Contact information |
| `SiteNavigationElement` | Website navigation |

### Software and development

| Schema type | Purpose |
| --- | --- |
| `SoftwareSourceCode` | GitHub repositories and source code |
| `SoftwareApplication` | Installable software |
| `WebApplication` | Browser-based applications |
| `MobileApplication` | Android and iOS applications |
| `APIReference` | API and function documentation |
| `ComputerLanguage` | Programming languages |
| `DigitalDocument` | Downloadable documentation |
| `DataDownload` | Downloadable datasets |
| `Dataset` | Structured data collections |
| `DataCatalog` | Dataset directories |

### Technical documentation

| Schema type | Purpose |
| --- | --- |
| `TechArticle` | Technical documentation |
| `Article` | General articles |
| `HowTo` | Installation and configuration tutorials |
| `HowToStep` | Individual tutorial steps |
| `HowToSection` | Groups of tutorial steps |
| `HowToDirection` | Specific instructions |
| `HowToTip` | Additional guidance |
| `HowToTool` | Required software or tools |
| `FAQPage` | Frequently asked questions |
| `Question` | Individual questions |
| `Answer` | Individual answers |
| `DefinedTerm` | Technical terminology |
| `DefinedTermSet` | Glossaries |
| `Blog` | Development blog |
| `BlogPosting` | Development articles and announcements |
| `QAPage` | Community questions and answers |

### Identity and authorship

| Schema type | Purpose |
| --- | --- |
| `Person` | Developer identity |
| `Organization` | Organizations and development teams |
| `Brand` | Project branding |
| `Role` | Contributor responsibilities |
| `ContactPoint` | Support channels |

### Education and qualifications

| Schema type | Purpose |
| --- | --- |
| `EducationalOccupationalCredential` | Qualifications |

### Media and assets

| Schema type | Purpose |
| --- | --- |
| `ImageObject` | Logos, screenshots and diagrams |
| `VideoObject` | Demonstrations and tutorials |
| `MediaObject` | Downloadable media |
| `AudioObject` | Audio tutorials and narration |
| `ImageGallery` | Screenshot galleries |

## Properties to generate automatically

| Category | Properties |
| --- | --- |
| Identity | `@id`, `@type`, `name`, `alternateName`, `url`, `identifier` |
| Description | `description`, `abstract`, `keywords`, `inLanguage` |
| Relationships | `mainEntity`, `mainEntityOfPage`, `isPartOf`, `hasPart`, `about`, `sameAs`, `subjectOf` |
| Authorship | `author`, `creator`, `contributor`, `maintainer`, `publisher` |
| Software | `codeRepository`, `programmingLanguage`, `runtimePlatform`, `targetProduct` |
| Application | `applicationCategory`, `operatingSystem`, `softwareVersion`, `softwareRequirements` |
| Distribution | `downloadUrl`, `installUrl`, `releaseNotes`, `fileSize`, `offers` |
| Licensing | `license`, `copyrightHolder`, `copyrightYear`, `isAccessibleForFree` |
| Dates | `dateCreated`, `datePublished`, `dateModified` |
| Media | `image`, `logo`, `screenshot`, `video`, `thumbnailUrl` |
| Documentation | `headline`, `articleSection`, `articleBody`, `wordCount` |
| Navigation | `breadcrumb`, `itemListElement`, `position`, `numberOfItems` |
| Tutorials | `step`, `tool`, `supply`, `totalTime`, `proficiencyLevel` |
| References | `citation`, `isBasedOn`, `relatedLink` |

Generate only applicable properties supported by repository metadata, project configuration or visible page content. Check the current Schema.org vocabulary, property domains and ranges before implementation. Omit unknown values; do not fabricate dates, authors, versions, ratings or other metadata. Use stable `@id` values to connect related entities. Valid structured data does not guarantee Google rich results or AI citations.
