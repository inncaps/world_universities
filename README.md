# World Universities

This repository contains the useful information about the world universities. This repository will contain this following information about the universities around the world,
 1. University Name and Location
 2. Short Description about the university
 3. Active Chancellor and Vice Chancellor Names and Contact information(Only if the official website exposed the contact information) 
 4. Faculties and Departments Information with Head of Departments and Staffs Information
 5. Available undergraduates and postgraduates information
 6. Module Information for every course in the department with relevant information

## Guidelines

Please read this guideline carefully before the contribution. 
 1. This will be used only for the educational purposes, So don't include any business related information here.
 2. Use the official website of the university to get more information for the related tags.
 2. Please don't include any wrong information here. If you can't confirm some information then, please leave that information.
 3. Check the JSON file before creating the Pull Request using some online tools(Eg: http://jsoneditoronline.org/)
 4. Please follow the PR template while sending the PR
 
## How to contribute to this project

You should get the university official website and use that to collect the relevant information. Please do not include any wrong information here. It will be used by most of the students for their studies. 
 1. Fork this repository to your GitHub account.
 2. Create new entry about the University
 3. Commit and Push your changes to your repository
 4. Create Pull Request to this repo(Please care about the PR guidelines)
 5. Thanks for your contribution and Don't forget to star the repository
 
### Folder Structure of the entries,

you want to follow this folder structure while creating the entries for the universities.

````
CountryName
|- UniversityName
|--- university_info.json
|--- faculties_departments.json
|--- modules.json
````


#### University Information JSON File

> Filename : `university_info.json`

Included Informations, 
 1. University Common Information
 2. Location of the university
 3. Contact Information 
 4. Main Officers of the university
 The JSON format for this file should be like,
 
````
{
    "university_name" : "NAME",
    "university_id" : "id",
    "web_url" : "university website URL",
    "motto" : "motto",
    "short_description" : "Descrtption",
    "location" : {
        "country" : "country_name",
        "state_name" : "state",
        "address_line_1" : "adress_1",
        "address_line_2" : "address_2",
        "postal_code" : "postal_code"
    },
    "contact_info" : {
        "telephone_1" : "telephone number",
        "telephone_2" : "telephone number",
        "mobile_number_1" : "mobile number",
        "fax" : "fax_number",
        "email" : "email"
    },
    "university_officers" : {
        "chancellor" : {
            "name" : "Chancellor Name",
            "email" : "Chancellor email",
            "contact_no" : "Chancellor Contact No"
        },
        "vice_chancellor" : {
            "name" : "Vice Chancellor Name",
            "email" : "Vice  Chancellor email",
            "contact_no" : "Vice Chancellor Contact No"
        },
        "deputy_chancellor" : {
            "name" : "Deputy Chancellor Name",
            "email" : "Deputy Chancellor email",
            "contact_no" : "Deputy Chancellor Contact No"
        },
        "registrar"  : {
            "name" : "Registrar  Name",
            "email" : "Registrar  email",
            "contact_no" : "Registrar  Contact No"
        }
    }
}
````

#### Faculty Information

> Filename : `university_info.json`

Included Informations, 
 1. University Common Information
 2. Faculties of the university
 3. Departments in the each faculty 
 4. Main Officers of the faculties and departments
 The JSON format for this file should be like,
 
````
{
    "university_name" : "NAME",
    "university_id" : "id",
    "faculties" : [
         {
            "faculty_name" : "Faculty Name",
            "web_url" : "Faculty URL",
            "dean_info" : {
                "name" : "Dean Name",
                "email" : "Dean email",
                "contact_no" : "Dean Contact No"
            },
            "departments" : [
          {
                    "department_name" : "Department Name",
                    "web_url" : "WEB URL",
                    "hod_info" : {
                        "name" : "HOD Name",
                        "email" : "HOD email",
                        "contact_no" : "HOD Contact No"
                    }
                }
            ]
        }
    ]
}
````

#### Course Module's Information

> Filename : `modules.json`

Included Informations, 
 1. University Common Information
 2. Undergraduate Degree Information
 3. Postgraduate Degree Information 
 4. Modules of the degrees.
 The JSON format for this file should be like,
 
````
{
    "university_name" : "NAME",
    "university_id" : "id",
    "undergraduate_degrees" : [
        {
            "degree_name" : "Degree Name",
            "duration" : "Course duration",
            "description" : "Short Description",
            "degree_section" : "Engineering",
            "modules" : [
              {
                    "module_name" : "Module name",
                    "module_id" : "Module Id",
                    "module_credit" : "Module Credit",
                    "semester" : 3,
                    "year_of_study" : "3rd Year"
                }
            ]
        }
    ],
    "postgraduate_degrees" : [
        {
            "degree_name" : "Degree Name",
            "duration" : "Course duration",
            "description" : "Short Description",
            "degree_section" : "Engineering",
            "modules" : [
                {
                    "module_name" : "Module name",
                    "module_id" : "Module Id",
                    "module_credit" : "Module Credit",
                    "semester" : 3,
                    "year_of_study" : "3rd Year"
                }
            ]
        }
    ]
}
````

### Pull Request Guidelines
If you are sending one PR for one university information then, follow this steps
 1. Please clearly indicate the university name in the PR title. 
 2. You can create multiple PR for each university information. In that case, mention the information type with university name. 
 3. If the PR doesn't contain the university name, then reviewers may reject the PR.
 
If you are sending one PR with multiple universities information, then follow this steps,
 1. Please clearly indicate the university name in the commit message. 
 2. You can create multiple commits for each university information. In that case, mention the information type with university name.
 3. If the commits don't contain the university name, then reviewers may reject the PR.
  
## License

[The MIT License (MIT)](https://github.com/Thuva4/Algorithms_Example/blob/master/LICENSE)
