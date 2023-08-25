<h1 align="center">Google Summer of Code 2023 <img src="https://media2.giphy.com/media/KB8MHRUq55wjXVwWyl/source.gif" width="50"></h1>

<p align="center"><i>A full report on my Google Summer of Code 2023 work with FOSSology</i></p>
<p align="center"><i>Project: "REST API Improvements" </i>  👨‍💻</p>

<p align="center">
        <img src="https://64.media.tumblr.com/c93f16953341ab06acd12b493659bdee/tumblr_mr68hhmVE11r5ikx8o1_400.gif" width="100">
</p>

![image](https://user-images.githubusercontent.com/66276301/188962690-5869b53c-99bb-4012-b13f-443832568f7e.png)

## Google Summer of Code 2023 🚩 Report: "REST API Improvements" 👨‍💻
<!-- 
![ViewCount](https://views.whatilearened.today/views/github/dushimsam/GSoC-2023.svg)
![GitHub](https://img.shields.io/github/followers/dushimsam?style=social)
![Twitter](https://img.shields.io/twitter/follow/dushimsam?style=social)
![GitHub Stars](https://img.shields.io/github/stars/dushimsam/GSoC-2023?style=social) -->

About me 👩‍💻

Hello, I'm **Samuel Dushimimana**, a proud graduate from the first class of Software Engineering and Embedded Systems at [**Rwanda Coding Academy**](http://rca.ac.rw/). With over 4 years of hands-on experience in building full stack applications, I'm thrilled to be an active member of the FOSSology community for Google Summer of Code 2023.

In this article am going to outline the details of my contributions as a reference of project completion during the 12 weeks of coding.

# 🌏 CONTRIBUTIONS Overview 

   During my participation in the Google Summer of Code (GSoC) program, I focused on implementing and enhancing eight key features within the project:

  1. #### License File View Management:
     I developed the REST APIs that tackled on extracting file contents and making the clearing decisions about associated licenses. This involved extracting, processing and highlighting 
     license information from the files.
  3. #### License Browser:
     I designed a set of APIs to facilitate the presentation of a tree view of files and their corresponding license details. Additionally, I implemented APIs that provided summary statistics 
     about the licenses associated with a particular uploaded content.
  4. #### Folder and Content Management:
     The task encompassed creating essential APIs for managing folder contents. This involved tasks such as retrieving removable contents from folders and unlinking contents from specific 
     parent folders.
  5. #### Admin Dashboard Management:
     I played a role in designing APIs that served different components of the Admin dashboard. These APIs provided data such as database metrics and job statistics, contributing to the 
     effective monitoring of the system.
  6. #### License Admin Management:
     I developed REST APIs that helped the system Admin to handle different operations on acknowledgments and standard comments related to licenses.
  7. #### CSV Operations:
     Another aspect of my work involved designing REST APIs for importing and exporting licenses and obligations using CSV files.
  8. #### Manual Scheduling of Operations:
     I created REST APIs that allowed administrators to schedule and execute various operations manually. 
  9. #### FOSSology API V2 configuration:
     I improved the configuration of the REST APIs to accommodate FOSSology API Version 2. This enhancement ensured compatibility with future versions and streamlined the process of 
     incorporating upcoming changes.

Let's dive deep into each category in more details to showcase all the contributions with the corresponding tests in screenshots where applicable, and the respective links to the Pull requests.


##  License File View Management :sparkles:

1. Setting the clearing decision for a particular file [#2460](https://github.com/fossology/fossology/pull/2460)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/c1dc616c-aa8e-44d1-8990-0be63503a0c5)
   
3. Setting the main license for the Upload [#2462](https://github.com/fossology/fossology/pull/2462)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/d991ebb3-cea3-4fbe-9752-1f7ec22bb112)
   
5. Removing the main license from the Upload [#2463](https://github.com/fossology/fossology/pull/2463)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/cccb6515-6f61-4fe0-9891-c84913cdce40)

6. License Decision Management (Add, edit & delete License Decision) [#2509](https://github.com/fossology/fossology/pull/2509)
   
   #### Request
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/36ca30e6-fa56-4dc3-85b1-f360f670b997)
   #### Response
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/7b037367-2d55-4fa5-a64c-2a376c19c2ba)

7. Get all main licenses for the the Upload [#2465](https://github.com/fossology/fossology/pull/2465)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/28e261ca-8448-4cc0-b63e-8c48c26622f3)

8. List all the license decisions for the item [#2470](https://github.com/fossology/fossology/pull/2470)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/98c3c925-01ee-4e00-97ef-e05b4a4e69dc)

10. Get the clearing history for a specific item [#2477](https://github.com/fossology/fossology/pull/2477)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/268214a0-2971-408e-b07a-de63c807e0ca)

11. Schedule the bulk scan [#2483](https://github.com/fossology/fossology/pull/2483)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/f964b884-fec9-4968-8c5c-3eef76981bde)

13. Handling three pointers functionality (moving from file to file). [#2480](https://github.com/fossology/fossology/pull/2480)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/2f562371-dc8d-48d8-ac44-c37b387da489)

14. Get the bulk history list of the upload & item [#2481](https://github.com/fossology/fossology/pull/2481)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/bafb2559-6154-4d5a-b613-81561ee998a0)

16. Get the positions to be highlighted in the contents of the file [#2484](https://github.com/fossology/fossology/pull/2484)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/0e1e3ccc-2cb3-4ab1-9d6b-23da04fddbc2)

17. Get the license tree-view of the upload and the item [#2492](https://github.com/fossology/fossology/pull/2492)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/ac8aa9f7-a0f1-4d87-92ad-a695a0fd9021)

##  License Browser :sparkles:

1. Get the clearing progress status of the upload [#2494](https://github.com/fossology/fossology/pull/2494)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/f5e2851e-a90e-49a1-887b-3f82d12d5ea9)

2. Get the scanned licenses for the upload [#2495](https://github.com/fossology/fossology/pull/2495)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/6ad8bd14-2ed0-4580-b76c-7a9f5fabeb8e)

3. Get the licenses histogram for the upload [#2497](https://github.com/fossology/fossology/pull/2497)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/9071acec-18a3-4d95-989e-0d763a334e86)

4. Get the edited licenses for the upload [#2498](https://github.com/fossology/fossology/pull/2498)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/a6fdf2dc-73d0-4a81-a146-a672ba635be9)

5. Get the licenses's count summary for the upload [#2499](https://github.com/fossology/fossology/pull/2499)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/a5a59a4f-d14b-41fa-9bad-b31d8b9c2791)

6. Get the licenses' reuse summary list for the upload [#2501](https://github.com/fossology/fossology/pull/2501)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/42ed7f7f-0469-4ae4-99e0-aec8add43887)

7. Get all the agents for the upload [#2502](https://github.com/fossology/fossology/pull/2502)

8. Get all the agents' revisions for the upload [#2506](https://github.com/fossology/fossology/pull/2506)

## License Admin Management :sparkles:

1. Get all the licenses admin acknowledgements [#2512](https://github.com/fossology/fossology/pull/2512)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/e7d0dc8c-37f1-4d4c-ac83-343c75a18f1d)

3. Manage (Add, Edit & toggle) license admin acknowledgment [#2516](https://github.com/fossology/fossology/pull/2516)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/366b748e-e289-45f8-a489-67db12f6ebf0)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/266b2b82-da5d-4783-bb6e-dbc00f9f0b55)

4. Get all the standard comments [#2517](https://github.com/fossology/fossology/pull/2517)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/b005ff6e-6e92-4220-8214-0a55dbe55dff)

5. Search and suggest license from the given reference text [#2524](https://github.com/fossology/fossology/pull/2524)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/271123b1-3595-4d78-b6ef-cd5dd5a2e0c1)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/e1ecc3dd-1b03-454c-8232-4da8680e49c6)

7. Verify a particular license as a new or a variant [#2528](https://github.com/fossology/fossology/pull/2528)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/8ee0e737-b47c-45e1-8461-bf688b7de2b9)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/06a3ca67-74e0-47d8-98f1-b39860827684)

9. Merge a license into an existing one [#2529](https://github.com/fossology/fossology/pull/2529)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/ddd53dcd-b3ce-4564-b60b-3aecbde9c161)

11. Manage (add, edit & toggle) the standard license comment [#2518](https://github.com/fossology/fossology/pull/2518)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/6b10eabe-9cbf-4bec-bb6f-e04edd455491)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/4e198ac6-3545-4035-9941-08f653ace9f8)

## Admin Dashboard Management :sparkles:

1. Get the database contents for the dashboard overview [#2530](https://github.com/fossology/fossology/pull/2530)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/4168a413-a3c8-4690-b5db-f1cb20ca6ced)

2. Get the database metrics for the dashboard overview [#2532](https://github.com/fossology/fossology/pull/2532)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/29f28e8b-5514-4169-88dd-eff57eb7d3ab)

3. Get the active queries for the dashboard overview [#2533](https://github.com/fossology/fossology/pull/2533)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/bd6d7964-877e-4fc8-adbb-50748fe329d4)

4. Get the disk space usage details for the dashboard overview [#2534](https://github.com/fossology/fossology/pull/2534)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/7868573f-8cbc-4466-b944-0d60c6caab3d)

5. Get the current PHP info details for the dashboard overview [#2535](https://github.com/fossology/fossology/pull/2535)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/e6f55d9c-00a6-4b81-93f1-282fd20c0d5a)

6. Get the server jobs for the Admin Dashboard [#2536](https://github.com/fossology/fossology/pull/2536)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/d235f31e-59ce-4d86-8db8-b269d5e512e1)

7. Show the summary statistics for all jobs [#2537](https://github.com/fossology/fossology/pull/2537)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/9bf7edab-0a10-4dcc-8433-810f62fd9133)

## Manual Scheduling of Operations :sparkles:

1. Get the scheduler options for the given operation [#2538](https://github.com/fossology/fossology/pull/2538)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/a1bb7034-323e-41f4-bf48-f771ce8a9d94)

2. Run the scheduler based on the given operation [#2539](https://github.com/fossology/fossology/pull/2539)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/d8629d8d-6e77-4b7b-86e3-dd72f40dc36e)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/daefcc86-2a90-4257-aa28-a549df5a3baf)

##  Folder and Content Management :sparkles:

1.  Get all the contents of the given folder [#2555](https://github.com/fossology/fossology/pull/2555)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/21de9279-501b-49b4-9892-0c02b8ec0f15)

3.  Get all removable contents for the given folder [#2551](https://github.com/fossology/fossology/pull/2551)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/5fc1f685-d4ef-412d-a4ba-636b7468f876)

4. Unlink the folder contents [#2552](https://github.com/fossology/fossology/pull/2552)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/15084ef2-778a-4092-bf96-4d392962c515)

## CSV Operations :sparkles:

 1. Export the lisenses-list as a CSV [#2562](https://github.com/fossology/fossology/pull/2562)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/36ca8062-42fc-4303-b06f-7c877495f5cb)
 2. Export the obligation-list as a CSV [#2574](https://github.com/fossology/fossology/pull/2574)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/2c37b800-9454-4b87-a14e-e2b04e560c55)
 3. Import the obligations from the CSV  [#2563](https://github.com/fossology/fossology/pull/2563)
    ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/ef77556f-715d-4ceb-b8b7-6f7b5a935624)

## FOSSology API V2 configuration :sparkles:

Redesigned the FOSSology API Config to support version 2 of REST APIs. Currently, the codebase was designed to support only version 1 of REST APIS which would be hard to introduce and utilize the new features offered by Version 2. [#2576](https://github.com/fossology/fossology/pull/2576)


## Documentation:📄

Throughout the 12 weeks of the GSoC period, I dedicated time to create weekly documentation to track and record updates. The weekly documentation of updates can be accessed [**here**](https://fossology.github.io/gsoc/docs/2023/rest/updates/samuel/2023-06-01)


<h1 align="center">👨🏻‍🏫 DELIVERABLES <img src="https://api.ezeelo.com/Scripts/QRCode/Done.gif" width="40"></h1>

| Tasks   | Planned | Completed     | Remarks    |
| :---:       |    :----:   |    :---:      |    :---:      |
| Completed all the APIs that were assigned to me on the task sheet | Yes       | :heavy_check_mark: | Some APIs need to be improved to meet the same standards and conventions for the V2 |
| I have improved the existing functionalities for the APIs to provide better service to the consumers. | Yes        | :heavy_check_mark:  |  |
| Improved the FOSSology API's configuration for easier integration with the REST API V2| Yes | :heavy_check_mark: | There's still a lot of work ahead to ensure that all the APIs follow the new standards and conventions for their requests and response models |
| Integrating the new APIs on the FOSSology UI side | NO (WAS OPTIONAL) | :x: | This is an ongoing work, as we will add more APIs in the future |
| Implementing the OAuth 2.0 | NO (WAS OPTIONAL) | :x: | We are looking how to use it with Slim |

## Future enhancements:🚀
In the pipeline are several exciting improvements to look forward to:

- #### Updating REST APIs to Version 2 Standards:
   Planning to update the existing REST APIs to align with the latest standards of Version 2. This update will ensure enhanced functionality, better usability, and improved compatibility with 
   evolving requirements.
- #### Integration of New APIs with FOSSology UI:
   There's still a work on integrating the newly developed APIs into the FOSSology user interface to finish the work of migrating FOSSology to Full-stack architecture.
- #### Performance Boost for APIs:
   There's a huge work on enhancing the performance of the APIs in terms of response time and speed, by incorparating different techniques like Caching.
- #### Enhanced Compatibility between the Architectures:
   There's a need in improving the compatibility between the current monolithic architecture and the new REST API architecture, such that the change on one end won't affect the performance of 
   the other. 

## Major Takeaways: 📚

- Work Proficiency in Remote culture.
- Getting started and contributing to Large Codebases with Confidence.
- Embracing the culture of Collaboration and Teamwork.
- Hands-On experience in Open Source Contribution.
- Growth in writing clean code and coding Proficiency.

## Links of work done: 🎯

### Pull Requests 🔗

- [FOSSology](https://github.com/fossology/fossology/pulls?page=1&q=is%3Apr+author%3Adushimsam+created%3A2023-05-01..2023-10-01)

# Let's get connected!

- [LinkedIn](https://www.linkedin.com/in/samuel-dushimimana-364a19194/)
- [GitHub](https://github.com/dushimsam)
- [Twitter](https://twitter.com/dushsamuel)

