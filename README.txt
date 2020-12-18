Our project name is "Mass Mailing Using C++"

For running this project following things are required:
1. Install the visual studio. This project is dependent on the visual studio. Note: Visual studio and Visual Studio code are two different softwares. You should go for the Visual studio.
	Use the following website to download - https://visualstudio.microsoft.com/downloads/

2. Install vcpkg package manager and integrate with the visual studio. This will make us easy to install any c++ library and use it in our project without depending upon the library. 
	for vcpkg go to this link -- https://github.com/microsoft/vcpkg to download the files and install it using the tutorial video - https://www.youtube.com/watch?v=URzE4V_kbb4

3. install the following library for this projects using vcpkg 
	vcpkg install boost
	vcpkg install openssl

4. install a file which is provided the website email architect and we have used this blog
	https://www.emailarchitect.net/easendmail/kb/vc.aspx?cat=0

5. A executable file is required which needs to be installed at your pc whose link is given below:
	https://www.emailarchitect.net/webapp/download/easendmail.exe

6. Note the first two lines of the code should be as your requirement. Note this program uses \\ for the change of directory which we use while changing the directory of the source code. 
	#define BODY_LOCATION "G:\\1. Mass Mailing System\\1. code working\\sending_mails_using-_CPP\\body.html" // Note the double back slash here. It is required
	#include "C:\vcpkg\downloads\tools\perl\5.30.0.1\c\lib\gcc\i686-w64-mingw32\8.3.0\include\stdfix.h"//SEARCH WHERE IS STDFIX.H AND COPY THE PATH HERE TO INCLUDE ok

7. Headers file required for the file are:
	EASendMailObj.tlh this is already included in the zip file 

After having this load the project in visual studio by 
File>New>Create New Project from Existing Code Files
A new popup will appear and for a question What type of project would you like to create?  ==> select Visual C++ and click on Next

Browse for the Project file location ==> Select the folder in which these file are located. 
Write the Project name ==> Mailing or any name you.  Other leave as it is and click Next again.

In the question How so you want to build the project? ==> Use Visual Studio
choose the Project Type as the == > Console application project, leave other as it is and click Next. 

After this for the question What settings do you want for the Debug configuration? ==> Leaving everything Empty and Click Next .
Then, Finally click the Finish key.

Now Run you project using Local Windows Debugger.
Enjoy ..... 

	