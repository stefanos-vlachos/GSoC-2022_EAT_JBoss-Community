GSoC submission 2022
===================

### GSoC-2022_EAT_JBoss-Community

----------

About the Team
-------------
The year 2022 marked the fifth consecutive participation of the Additional Testsuite research project in the Google Summer of Code. This year the team comprised of Panagiotis Soritopoulos (Ph.D. Candidate in the Department of Informatics and Telecommunications) and Stefanos Vlachos (graduate student of the Department of Informatics and Telecommunications).

About EAT
-------------

EAT is a testsuite to develop tests against infinite number of JBoss servers. It’s an innovative tool because it’s creating the test once and testing with any version of the tested software.The idea behind the project, the AT (Additional Testsuite) structure, covers a wide variety of new features that could be added to it. One of them, is the addition of a CI (Continuous Integration) tool to perform some automated testing operations. EAT is available for a number of server configurations and a CI pipeline can be built using the maven tool.


#### Advantages of EAT

1. Writing the tests once and testing against infinite number of Application Servers.
2. Having all the tests at one place.
3. Comparison of the servers based on the testsuite.
4. Guarding against regression.
5. Faster convergence among the servers.
6. Comparison of the servers based on tests of the past and the present.
7. Addition of tests with possible future features that are not at the moment available.
8. It makes possible to push a testcase of a fix regarding a specific component of the server, without the component version to have been updated at the server pom.


Our 2022 Contribution
-------------

This year, our team’s goals were:
1. to extend the functionality of the Additional Testsuite implementation to provide support for testing the latest version of JBoss Community Server to be released
2. to dynamically create/build multi-version Android projects which would be checked on the device, and
3. to create of a multi-version Android application where proposals and Additional Testsuite-related function/program descriptions would be displayed.


Project Timeline - Results
------------------------------

The implementation of the project lasted from June 2022 to November 2022 (Large Size Project) and the timeline
was envisaged as follows:

### 1st Phase (June 2022 - July 2022)

During the 1st phase of GSoC 2022 a snapshot was added to the EAT project for testing the latest version of JBoss Community Server.

In more detail, the 27.0.0.Final version of the [Wildfly](https://github.com/wildfly/wildfly) server was added to EAT ([COMMIT 1](https://github.com/stefanos-vlachos/EAT/commit/389dbd3bdad5a37db0bd78a964d9b71a5c8a6a3c), [COMMIT 2](https://github.com/stefanos-vlachos/EAT/commit/252bff10dbd7dbe6743154e01eac4426d28030d1)).

### 2nd Phase (July 2022 - September 2022)

During the 2nd phase of this project, new multi-version Android projects were added to EAT. In EAT there is already a basic android multi-version example. This was extended with other open source android projects, demonstrating how EAT can be used to support multi-version real life android projects.

The open source projects that were selected and finally integrated into EAT can be found in https://github.com/topics/android-project and are the following:
- BloodBank ([GITHUB REPO](https://github.com/stefanos-vlachos/BloodBank), [PULL REQUEST](https://github.com/EAT-JBCOMMUNITY/EAT/pull/221))
- Elegant_Calculator ([GITHUB REPO](https://github.com/stefanos-vlachos/Elegant_Calculator), [PULL REQUEST](https://github.com/EAT-JBCOMMUNITY/EAT/pull/223))
- My_Companion ([GITHUB REPO](https://github.com/stefanos-vlachos/My_Companion), [PULL REQUEST 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/234), [PULL REQUEST 2](https://github.com/EAT-JBCOMMUNITY/EAT/pull/238))
- TruthDare ([GITHUB REPO](https://github.com/stefanos-vlachos/TruthDare), [PULL REQUEST 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/233), [PULL REQUEST 2](https://github.com/EAT-JBCOMMUNITY/EAT/pull/237))
- ThemeSample ([GITHUB REPO](https://github.com/stefanos-vlachos/ThemeSample), [PULL REQUEST 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/230), [PULL REQUEST 2](https://github.com/EAT-JBCOMMUNITY/EAT/pull/239))
- voxRec ([GITHUB REPO](https://github.com/stefanos-vlachos/voxRec), [PULL REQUEST 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/235), [PULL REQUEST 2](https://github.com/EAT-JBCOMMUNITY/EAT/pull/236))
- ImageBox ([GITHUB REPO](https://github.com/stefanos-vlachos/ImageBox), [PULL REQUEST](https://github.com/EAT-JBCOMMUNITY/EAT/pull/232))
- MyCamera ([GITHUB REPO](https://github.com/stefanos-vlachos/MyCamera), [PULL REQUEST](https://github.com/EAT-JBCOMMUNITY/EAT/pull/231))
- JKSLinks ([GITHUB REPO](https://github.com/stefanos-vlachos/JKSLinks), [PULL REQUEST 1](https://github.com/EAT-JBCOMMUNITY/EAT/pull/243))


### 3rd Phase ( September 2022 – November 2022)

During the 3rd and final stage of our team’s participation in the GSoC 2022 an Android application, named [**EAT-PROPOSALS**](https://github.com/stefanos-vlachos/EAT-PROPOSALS), was developed and finally integrated ([PULL REQUEST](https://github.com/EAT-JBCOMMUNITY/EAT/pull/264)) into the EAT project. 

#### About EAT-PROPOSALS
------------------------

The idea behind the EAT-PROPOSALS app was to develop an application that would enable users to Upload, View and Download proposals and Additional Testsuite related function/program descriptions.

In more detail, the EAT-PROPOSALS app meets the following requirements:
- A user should be able to create a new account filling and submitting a Create an account form
> After a user submits a Create an account form, a verification email should be sent to the user so that the given email addres sis verified
- A user that has successfully created an account should be able to sign in the app filling and submitting a Login form
- Signed In users should be able to upload a selected file or folder form the internal storage of the mobile device
> - The platform should allow users to upload only certain types of files, that are defined in the database of the app
> - When a file/folder is uploaded, it should be placed in approval state and it should not be visible on the app until the administrator of the app approves it
- Every user, Signed In or not Signed In, should be able to view a selected file among a list of uploaded and approved files/folders
- Every user, Signed In or not Signed In, should be able to download a selected file/folder

#### Tech Stack & Requirements
------------------------------

EAT-PROPOSALS is an Android application developed on the **IntelliJ IDE** using the **Java** programming language. It was compiled using the **Android SDK 32.0.0** and requires an **Android version ≥ 7.0** and an **Android SDK ≥ 30**. 

[**Firebase**](https://firebase.google.com/), which is an app development platform that provides numerous services and extensions for building and growing applications including Android apps, forms the backbone of the application and enables:
  1. the authentication of registered users
  2. the storage of uploaded files/folders

[**Mailgun**](https://www.mailgun.com/), which is an E-mail delivery service, and the [**Retrofit**](https://github.com/square/retrofit) library were utilized so that the administrator of the app gets notified via E-mail for new uploads on EAT-PROPOSALS.

#### EAT-PROPOSALS on Google Play Store
-------------------------------
EAT-PROPOSALS has been set up so that it is eventually published on **Google Play Store**.


 OTHER RESOURCES
----------------------------

- [EAT-PROPOSALS on GitHub](https://github.com/stefanos-vlachos/EAT-PROPOSALS)
- [EAT Project on GitHub](https://github.com/EAT-JBCOMMUNITY/EAT)
- [EAT Workshop](https://www.dropbox.com/s/bebhyd1iz7cg1i2/EAT_WORKSHOP.odt?dl=0)
- [Our GSoC 2022 Proposal](https://summerofcode.withgoogle.com/programs/2022/projects/k3hMrNAM)
- [Panagiotis Sotiropoulos on GitHub](https://github.com/EAT-JBCOMMUNITY)
