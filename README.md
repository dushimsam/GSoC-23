<h1 align="center">Google Summer of Code 2023 <img src="https://media2.giphy.com/media/KB8MHRUq55wjXVwWyl/source.gif" width="50"></h1>

<p align="center"><i>A full report on my Google Summer of Code 2023 work with FOSSology</i></p>
<p align="center"><i>Project: "REST API and UI improvements" </i>  👨‍💻</p>

<p align="center">
        <img src="https://64.media.tumblr.com/c93f16953341ab06acd12b493659bdee/tumblr_mr68hhmVE11r5ikx8o1_400.gif" width="100">
</p>

![image](https://user-images.githubusercontent.com/66276301/188962690-5869b53c-99bb-4012-b13f-443832568f7e.png)

## Google Summer of Code 2023 🚩 Report: "REST API and UI improvements" 👨‍💻
<!-- 
![ViewCount](https://views.whatilearened.today/views/github/dushimsam/GSoC-2023.svg)
![GitHub](https://img.shields.io/github/followers/dushimsam?style=social)
![Twitter](https://img.shields.io/twitter/follow/dushimsam?style=social)
![GitHub Stars](https://img.shields.io/github/stars/dushimsam/GSoC-2023?style=social) -->

About me 👩‍💻

I am **Samuel Dushimimana**, a graduate from the first cohort in Software Engineering and Embedded Systems at [**Rwanda Coding Academy**](http://rca.ac.rw/) with more than 4 years of experience in building full stack applications. I'm so excited to be a part of FOSSology community in Google Summer of Code 2023.

In this article am going to outline the details of my contributions as a reference of project completion during the 12 weeks of coding.

# 🌏 CONTRIBUTIONS Overview 

During this period i have been working on specifically on 8 features:

  1. License File View Management: This included the tasks of extracting the contents of the files, and taking the decisions of the licenses associated with it.
  2. License Browser: This included designing the appropriate APIs for serving all the details regarding the tree view of files and the licenses associated with a specific upload.
  4. Folder and Content Management: The tasks included desgining the missing APIs for managing the folder contents such as retrieving removable contents, and unlinking contents from specific parent folders.
  5. Admin Dashboard Management: This task included desigining the APIs responsible for serving the full components of the dashboard such as database metrics, jobs statistics etc.
  6. License Admin: This task included desiging the REST APIs enabling the Admin to manage the ackngoweledments and the standard comments.
  7. CSV Operations: The task included desiginnig the REST APIs for importing and exporting the Licenses, and obligations.
  8. Scheduler: The task included the REST APIs to enable the Admin to get different operations and the gives them the capability of runing specific operations in the project. 
  9. FOssology API V2 configuration: The task included restructuring the REST APIs configuration such that It is able to serve the Version 2 of the REST APIs.


Let's dive into each category in details to showcase all the contributions with the corresponding tests in screenshots where possible and the respective links to the Pull requests.

##  LICENSE FILE VIEW MANAGEMENT :sparkles:

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

##  LICENSE Browser Management :sparkles:

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

###  LICENSE ADMIN Management :sparkles:

1. Get all the licenses admin acknowledgements [#2512](https://github.com/fossology/fossology/pull/2512)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/e7d0dc8c-37f1-4d4c-ac83-343c75a18f1d)

3. Manage (Add, Edit, Remove & toggle) license admin acknowledgment [#2516](https://github.com/fossology/fossology/pull/2516)
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

#### Admin Dashboard Management:

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

#### Manual Operation Scheduling Management

1. Get the scheduler options for the given operation [#2538](https://github.com/fossology/fossology/pull/2538)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/a1bb7034-323e-41f4-bf48-f771ce8a9d94)

2. Run the scheduler based on the given operation [#2539](https://github.com/fossology/fossology/pull/2539)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/d8629d8d-6e77-4b7b-86e3-dd72f40dc36e)
   ![image](https://github.com/dushimsam/GSoC-23/assets/66276301/daefcc86-2a90-4257-aa28-a549df5a3baf)

