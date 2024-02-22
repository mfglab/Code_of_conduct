# Fair Principles

The [‘FAIR Guiding Principles for scientific data management and stewardship’](https://www.nature.com/articles/sdata201618) were published in 2016 to serve as guidelines for improving the **F**indability, **A**ccessibility, **I**nteroperability, and **R**eusability of scientific data. The principles emphasize machine-actionability because the increase in volume, complexity and creation speed of data made humans increasingly rely on computational support to deal with the data. The ultimate goal of FAIR is to drive science and the production of new datasets, as it allows researchers to build on existing comprehensively annotated studies with the intention of accelerating the scientific discoveries. 

Fair data principles were developed to improve data integrity and should be used as a guide for the production and publishing of data. The use of these principles should also be expanded to the algorithms, tools and workflows in the laboratories that produced the data as well as to the digital environment in which the data is located. While researchers need to be able to find and understand published datasets, computers need to handle (big) data depending on the intended use case. Thus, the FAIR principles also aim to improve the machine-readability of datasets for autonomous processing, while preserving human-readability.

### Findable

- [F1. (Meta)data are assigned a globally unique and persistent identifier](#f1-metadata-are-assigned-a-globally-unique-and-persistent-identifier)
- [F2. Data are described with rich metadata (defined by R1 below)](#f2-data-are-described-with-rich-metadata-defined-by-r1-below)
- [F3. Metadata clearly and explicitly include the identifier of the data they describe](#f3-metadata-clearly-and-explicitly-include-the-identifier-of-the-data-they-describe)
- [F4. (Meta)data are registered or indexed in a searchable resource](#f4-metadata-are-registered-or-indexed-in-a-searchable-resource)

### Accessible

- [A1. (Meta)data are retrievable by their identifier using a standardized communications protocol](#a1-metadata-are-retrievable-by-their-identifier-using-a-standardised-communications-protocol)
  - [A1.1 The protocol is open, free, and universally implementable](#a11-the-protocol-is-open-free-and-universally-implementable)
  - [A1.2 The protocol allows for an authentication and authorisation procedure, where necessary](#a12-the-protocol-allows-for-an-authentication-and-authorisation-procedure-where-necessary)
- [A2. Metadata are accessible, even when the data are no longer available](#a2-metadata-are-accessible-even-when-the-data-are-no-longer-available)

### Interoperable

- [I1. (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation](#i1-metadata-use-a-formal-accessible-shared-and-broadly-applicable-language-for-knowledge-representation)
- [I2. (Meta)data use vocabularies that follow FAIR principles](#i2-metadata-use-vocabularies-that-follow-fair-principles)
- [I3. (Meta)data include qualified references to other (meta)data](#i3-metadata-include-qualified-references-to-other-metadata)

### Reusable

- [R1. (Meta)data are richly described with a plurality of accurate and relevant attributes](#r1-metadata-are-richly-described-with-a-plurality-of-accurate-and-relevant-attributes)
  - [R1.1. (Meta)data are released with a clear and accessible data usage license](#r11-metadata-are-released-with-a-clear-and-accessible-data-usage-license)
  - [R1.2. (Meta)data are associated with detailed provenance](#r12-metadata-are-associated-with-detailed-provenance)
  - [R1.3. (Meta)data meet domain-relevant community standards](#r13-metadata-meet-domainrelevant-community-standards)


![FAIR Data Principles](./../img/FAIR.jpg)

## Detailed explanation

### Findable

The first step in (re)using data is to find it, so metadata and data should be easy to find for both humans and computers, including machine-readable metadata that are essential for automatic discovery of your datasets and services.

#### F1. (Meta)data are assigned a globally unique and persistent identifier

Principle F1 is arguably the most important because it will be hard to achieve other aspects of FAIR without globally unique and persistent identifiers. A persistent identifier (PID) is a long-lasting reference, normally used in the context of digital resources accessible over the internet, in this case your dataset. Globally unique and persistent identifiers remove ambiguity of your published data by assigning a unique identifier to every element of metadata and every concept/measurement in your dataset. Many data repositories will automatically generate globally unique and persistent identifiers to deposited datasets. Identifiers can also help other people understand exactly what you mean, and they allow computers to interpret your data in a meaningful way. They are also essential to the human-machine interoperation that is key to the vision of Open Science. In addition, identifiers will help others to properly cite the work when reusing your data.

A PID you have probably already heard of as most biological journals assign them to manuscripts, is the Digital Object Identifier (DOI). Your personal 16-digit (ORCID) or the accession number of your RNASeq dataset on GEO also represent examples for PIDs

#### F2. Data are described with rich metadata (defined by R1 below)

To enable (automatic) findability of your dataset, it is essential for humans and computers to understand its content. Taking this into account metadata can (and should) be generous and extensive, including descriptive information about the context, quality and condition, or characteristics of the data. The rationale behind this principle is that someone should be able to find data based on the information provided by their metadata, even without the data’s identifier. As such, compliance with F2 helps people to locate your data, and increase re-use and citations. Rich metadata implies that you should not presume that you know who will want to use your data, or for what purpose.

#### F3. Metadata clearly and explicitly include the identifier of the data they describe

The metadata and the dataset they describe are usually separate files. The association between a metadata file and the dataset should be made explicit by mentioning a dataset’s globally unique and persistent identifier (F1) in the metadata. 
Even though your dataset might not have been published, and archived subsequently, the PID included in the metadata can link you as the responsible contact person for the dataset. Thereby, the PID can still help other researchers to find your data and you in increasing your reach.

#### F4. (Meta)data are registered or indexed in a searchable resource

Identifiers and rich metadata descriptions alone will not ensure ‘findability’ on the internet. Perfectly good data resources may go unused simply because no one knows they exist. If the availability of a digital resource such as a dataset, service or repository is not known, then nobody (and no machine) can discover it. There are many ways in which digital resources can be made discoverable, including indexing.
Repositories ensure that metadata of a submitted dataset are filed in a machine-readable format to enable indexing. The indices of your metadata are used to efficiently search and find datasets.

### Accessible

Once users find your data, they need to know how they can access it, possibly including authentication and authorisation.

#### A1. (Meta)data are retrievable by their identifier using a standardised communications protocol

Standardized communication protocols, in combination with persistent identifiers, can guarantee access to your datasets, as links are maintained by the identifier providers. Examples of such protocols are http(s) or ftp(s). Accordingly, the combination of protocol and PID could look like <ins><https://doi.org/10.1000/182></ins>. Protocols with poor documentation or elements that need human assistance should be avoided, as these lead to hurdles in accessing data. For highly sensitive data it can be an option to provide an email or telephone number of a contact person, as fully mechanized protocols cannot guarantee secure access.

#### A1.1 The protocol is open, free, and universally implementable

To maximize data reuse, the protocol should be free (no-cost) and open (-sourced) and thus globally implementable to facilitate data retrieval. Anyone with a computer and an internet connection can access at least the metadata. Hence, this criterion will impact your choice of the repository where you will share your data. As a researcher, you can maximize the reuse of your data if you share your data with repositories that follow these criteria. Avoid proprietary and non-standard protocols

#### A1.2 The protocol allows for an authentication and authorisation procedure, where necessary

At this point it is very important to differentiate between "accessible" and "open" data. The "A" in FAIR does not imply that you are required to grant free access for everyone to your data, but rather to specify conditions under which the data are accessible. Even protected data are FAIR, if requirements were defined on how the data can be retrieved. Ideally, accessibility is specified in such a way that a machine can automatically understand the requirements, and then either automatically execute the requirements or alert the user to the requirements. It often makes sense to request users to create a user account for a repository. This allows to authenticate the owner (or contributor) of each dataset, and to potentially set user-specific rights. Hence, this criterion will also affect your choice of the repository where you will share your data.

An example for this case is a private non-visible repository on [GitLab][kb-DataHub], accessible only to defined users. As owner of the GitLab repository, you can select these users and researchers simply identify using the GitLab sign-in. Accordingly, the mechanism to allow users to identify themselves, belongs to the responsibility of the infrastructure provider.

#### A2. Metadata are accessible, even when the data are no longer available

Datasets tend to degrade or disappear over time because there is a cost to maintaining an online presence for data resources. When this happens, links become invalid and users waste time hunting for data that might no longer be there. Metadata and actual datasets should be stored in separate files because storing the metadata generally is much easier and cheaper. In this way, your metadata can and should persist even when the dataset was archived or is no longer supported. Researchers and infrastructure providers can thereby ensure that a link to responsible contact persons remains available, that researchers do not waste time searching for the data.

### Interoperable

To make your data reusable, it needs to interoperate with applications or workflows for analysis, storage, and processing.

#### I1. (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation

Besides other researchers, with whom you want to discuss and exchange your discoveries, your data can be processed by machines. This should be possible without human assistance or any additional algorithms, tools, or mappings specifically developed for this use case. Interoperability typically means that each computer system at least has knowledge of the other system's data exchange formats. Hence, using a good data model, to describe and structure your (meta)data and using commonly used controlled vocabularies, ontologies, and thesauri, each with globally unique PIDs, strongly supports you in generating interoperable data that can be found automatically. This holds especially true for metadata, as they contextualize your dataset and in the ideal case avoid any kind of questions or confusion.

#### I2. (Meta)data use vocabularies that follow FAIR principles

When we are describing data or metadata, we often use vocabularies that provide the terms or concepts that are adequate to represent their content. However, if we use vocabularies in our data or metadata, we should make sure that they are also FAIR in their own right so that others, humans or machines, can find, access, interoperate and reuse them. The controlled vocabulary used to describe datasets needs to be documented and resolvable using globally unique and persistent identifiers. This documentation needs to be easily findable and accessible by anyone who uses the dataset, e.g., by a URL included in your metadata.

#### I3. (Meta)data include qualified references to other (meta)data

Datasets are not static since they can evolve through extension by additional data or analyses by new algorithms. In such cases you generate newer versions of your data, which need to be stated as such by qualified references. Qualified references are cross-references that explain their intent, meaning in our example that characterizing V1 as the previous version of V2 of your dataset is a much more qualified reference than simply describing the two versions as related. Correspondingly, you should provide as many meaningful links as possible, preferably via PIDs, between datasets that build on other datasets, additional datasets needed to complete a dataset, or complementary information stored in a different dataset.

### Reusable

The ultimate goal of FAIR is to optimize the reuse of data. To achieve this, metadata and data should be well-described so that they can be replicated and/or combined in different settings.

#### R1. (Meta)data are richly described with a plurality of accurate and relevant attributes

It will be much easier to find and reuse data if there are many labels attached to the data. Principle R1 is related to F2, but R1 focuses on the ability of a user (machine or human) to decide if the data is actually USEFUL in a particular context. To make this decision, the data publisher should provide not just metadata that allows discovery, but also metadata that richly describes the context under which the data was generated. Moreover, R1 states that the data publisher should not attempt to predict the data consumer’s identity and needs. As author of your dataset you cannot expect other researchers to be familiar with your methods or domain. Therefore, you should be as generous as possible in providing metadata and even include information that seems irrelevant to you.

As an infrastructure provider you should give researchers the option to include a variety of metadata, including optional and free-text fields. Exemplary questions that need to be answered by the metadata are:

- Who created the data?
- When was the data created and/or published?
- How was the data generated?
- How was the data processed?
- Are there any limitations other users should be aware of?
- ...

#### R1.1. (Meta)data are released with a clear and accessible data usage license

You should clearly describe the usage rights for your data and include it in your metadata, as ambiguity could severely limit its reuse. Hence, the conditions under which the data can be used should be clear to machines and humans and can, e.g., be represented in form of a license. For scientific data, [Creative Commons licenses][ext-CreativeCommons] are commonly used.

#### R1.2. (Meta)data are associated with detailed provenance

For others to reuse your data, they should know where the data came from (i.e., clear story of origin/history, see R1), who to cite and/or how you wish to be acknowledged. Include a description of the workflow that led to your data, this includes a human- and machine-readable description of persons who collected the data, how has it been processed, if the data has been published before or if it contains data from someone else that you may have transformed or completed. This information must be linked via PIDs. Always keep in mind that other researchers want to be just as much acknowledged for their work as you.

#### R1.3. (Meta)data meet domain-relevant community standards

Researchers find it easiest to reuse data, if they are familiar with the type of data, file formats (well-established and sustainable), how the (meta)data is organized, and if commonly used vocabularies and ontologies are integrated. If community standards or best practices for data archiving and sharing exist, they should be followed. For instance, many communities have minimal information standards (e.g., MIAME, MIAPE). FAIR data should at least meet those standards.  Other community standards may be less formal, but nevertheless, publishing (meta)data in a manner that increases its use(ability) for the community is the primary objective of FAIRness. In some situations, a submitter may have valid and specified reasons to divert from the standard good practice for the type of data to be submitted. This should be addressed in the metadata.


All the above stated applies to data (or any digital object), metadata (information about that digital object), and infrastructure.