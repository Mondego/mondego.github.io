# About The Site
This is the official website of [Mondego Research Group](https://mondego.github.io/) at [University of California, Irvine (UCI)](https://ics.uci.edu/).
<br>
This website is powered by [Jekyll](https://jekyllrb.com/) and some Bootstrap, Bootwatch. The design is adopted from
[Allan Lab](https://github.com/mpa139/allanlab). 

## How to Update Website Contents

The site contains a **[_data](/_data/)** directory to store all its content.
The directory contains several **_.yml_** files to store different types of contents as mentioned below:


* Members & Alumni
* Research Domains & Publications
* Projects
* Software & Datasets
* Photos

Follow the steps to learn how to add/update each type of content.

* ### Add/Update Members & Alumni
To add a new member, it requires to append the following entry in **[members.yml](/_data/members.yml)** file. 
In generally, the entry should be at the  end of the file.<br>
However, it can be placed anywhere to maintain the order/serialization of members. <br>
Similarly, to add a new alumni just add an entry to the ***[alumni.yml](/_data/alumni.yml)*** file.

``` yml
- name: 
  photo: dummy_dp.png
  current_position:
  current_organization:
  email: 
  # Homepage can be personal website/ Google Scholar/ LinkedIn or any other authenticated educational profiles such as Resarch_Gate, GitHub etc.
  # However, keep it professional, do not add any social network account.
  homepage:
  # The value of number_educ varies between 1 to 5. Depending on the value, change the education1, education2 and so on.
  number_educ: 2
  education1:
  education2:  
```

* ### Add/Update Research Domain

To add a Research Domain, it requires to append the following entry in the **[domains.yml](/_data/domains.yml)** file.

```yaml
# serial no
- domain_name: Code Search
  domain_id: code_search
```

* ### Add/Update Publications

To add a publication, it requires to append the following entry at **the top** of **[publications.yml](/_data/publications.yml)** file.

```yaml
  # Mandatory field
- title: "" 
  # Mandatory field. List of all authors, separated by comma 
  authors: 
  # Mandatory field
  # Add the full booktitle as DBLP provides and includes the page numbers and publisher as a single string . 
  # (For journal include volume, page number other information )
  booktitle: 
  # Mandatory field as the (filtering requires year)
  year: 2025
  # Mandatory field. Must include least one domain_id (provided in _data/domains.yml)
  # If the paper falls in multiple research domains, add multiple domain_id separated by 'space'
  # The domain_id must be presented in the domains.yml file before adding into the publications.
  domain_id:
  # Mandatory field, type must be one of these 4 (Journal, Conference, Arxiv, Thesis)
  type:
  # If available, provide the paper pdf link
  pdf:
  # If available, provide Digital Library (DL) url
  url:
  # If available, provide digital object identifier as provided in DBLP  
  doi:
  # If available, provide the paper artifacts link, such as source code GitHub link, or provided dataset link
  code_link:
```

* ### Add Projects

To add a new project, it requires to create a **_YYYY-MM-DD-post-short-title.md_** 
file inside the **[_projects](/_projects/)** directory.<br>
The **_file name must be_** in **YYYY-MM-DD-project-short-title.md** format.<br>
Before writing the project contents, the following entry must be made at the top of the **_YYYY-MM-DD-project-short-title.md_** file.


```yaml
---
layout: projects # Mandatory field 'projects'
title:
subtitle:
author: 
cover-img: /images/projects/img_file
thumbnail-img: /images/projects/img_file
share-img: /images/projects/img_file
tags: [tag_name]
permalink: /YYYY-MM-DD-project-short-title/
comments: false
---

# project contents ...

```

* ### Add Photos

To add a new photo, it requires to append the following entry in **[photos.yml](/_data/photos.yml)**.
<br> However, to place the photo in  specific position, make the entry in exact serialization order.

```yaml
# serial no
- title: photo description
  image: photo_file_name.jpg
```
