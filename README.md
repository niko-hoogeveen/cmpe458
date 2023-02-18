# cmpe458

Phase 1: Scanner Files

Phase 2: Parser Files 
  - parser.ssl file has been uploaded, and is pretty much good to go. Still could modify 'ValueOrQuby' rule, but honestly at this point I don't care 
  - Instructions for running the parser:
    - Copy and paste parser.ssl code into your VM's parser.ssl file
    - Open the terminal and cd into ../ptsrc/parser
    - Run the following command:
          make
    - Now go into your parser.def file, and copy and paste the contents into parser.pt
    - Run the following commands:
          cd ..
          ssltrace "ptc -o2 -t2 -L lib/pt test/test.pt" lib/pt/parser.def -e
    - *Note: You must change the name of "test.pt" to the specific file name of the test you are trying to run. Optionally, you can copy and paste the contents of the test are running to a test.pt file on your VM, that way you dont have to crowd your VM with a shit ton of files. See phase 2 test suite folder in this git for a complete test suite file with all the tests that must be run. 
  - Instructions for creating test files:
   - Make a .txt file, .eOutput file, and .pt file for each test case as seen in tutorial 3.
   - Make sure the 3 files for each test are named the same except for the . exstension 
   - add nikos tests from the master to each corresponding .pt file.
   - Run each file to get its token trace as seen above.
   - Take that output and put it into the eOutput file for that test.
   - Document that test in the corresponding .txt file.
    
