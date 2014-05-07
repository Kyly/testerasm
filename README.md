CSE 30 tester
=================
######Version .02 of pa# tester for CSE 30.

HOW TO INSTALL TESTER
---------------------
1. *(optional)* Make a directory named scripts to hold this script or any others
  you may have.
  ````bash
  cd ~
  mkdir scripts
  ````
2. *(MUST DO)* Go into your script file then run the following command.
  ````bash
  cd scripts
  curl -#L https://github.com/Kyly/testerasm/archive/master.tar.gz \
  | tar zx && mv testerasm-master/tester . && chmod +x tester && \
  rm -rf testerasm-master
  ````
3. *(optional)* If you would like to run the tester without having to type
  the path (ex. ~/scripts/tester) you can add the the path to your .bash_profile
  be doing the following.

  ````bash
  'export PATH=$PATH:/home/solaris/ieng9/cs30x/cs30xxx/scripts' >> ~/.bash_profile
  ````
  If for some reason this gives you an error just open ~/.bash_profile in 
  vim and paste the export command somewhere in the middle.

  *"cs12xxx" will need to be changed to your own profile id.*

HOW TO USE TESTER
-----------------
  Go into your pa# directory that you wish to test and run the following command.
  ````bash
  tester pa# pa#test testfile
  ````
  "testfile" is a file you will need to make for each homework assignment.
  A small sample file is included in the git repository.

  The solution program (pa#test) and your program (pa# or whatever) will both 
  be run then both will be opened in vimdiff for comparison. The file will 
  show "TEST" followed by a number indicating which test you are looking at. 
  The test number correspond to the line number of the test in you test file.

  *"mine" is the name of the document that contains your test cases*
  *"sol" is the name of the document that contains the solutions test cases*

