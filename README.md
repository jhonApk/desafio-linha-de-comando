WELCOME
--------------------------------------------------------------------------------
Congratulations, you opened the README.txt file! You're well on your way to
becoming a command line ninja.

WHAT IS THIS?
--------------------------------------------------------------------------------

OK! Let's get started.

1. (B) Extract the "challenges.tar.gz" archive; you'll need its contents to
   solve some of the challenges.
      - Command: tar -xzvf challenges.tar.gz

2. (B) Change your working directory to the "challenges" directory that was
   created when you extracted "challenges.tar.gz"
	- Command: cd ./challenges

3. (B) List the contents of the "challenges" directory.
	- Comand: ls (lista o conteudo)
		- ls -a (lista o conteudo com pastas ocultas)
		- ls -l(lista com detalhe de perminssão, tamanho, data)

4. (B) Create a new directory named "foo".
	- Command: mkdir foo (cria o diretorio)

5. (I) Create a new directory named "foo/bar/1/2/3"
	- Command: mkdir -p foo/bar/1/2/3 (cria os diretorios
)
6. (B) Remove the directory "foo" and all of its contents
	- Command: rm -rf foo

7. (B) Print the text "Hello World".
	- Command: echo "Hello world"

8. (B) Create a file named "hello.txt" that contains the text "Hello World".
	- Command: echo "Hello World" > hello.txt && printf "Hello World" > hello.txt

9. (B) Create an empty file named "empty.txt"
	- Commmand: touch empty.txt

10. (B) Remove the file "empty.txt"
	- Command: rm empty.txt

11. (I) Find a second way to solve challenge 9.
	- Command: unlink empty.txt

12. (I) Find a third way to solve challenge 9.
	- Command: find . -name "empty.txt" -delete

13. (B) Copy "hello.txt" and name the copy "goodbye.txt".
	- Command: cp hello.txt goodbye.txt

14. (B) Rename "goodby.txt" to "hello_copy.txt".
	- Command: mv goodbye.txt  hello_copy.txt

15. (I) Prove that the contents of "hello.txt" and "hello_copy.txt" are
    identical.
	- Command: diff -s hello.txt hello_copy.txt
 
16. (B) Concatenate the contents of "hello.txt" and "hello_copy.txt" and store
    the result in a file named "2_hellos.txt".
	- Command: cat hello.txt hello_copy.txt >> 2_hellos.txt

17. (B) Get the full path of your present working directory ("challenges").
	- Command: navegue com cd ./challenges e use o comando  pwd 

18. (B) List the contents of the "challenges" directory (like challenge 3), but
    show the permissions for each file.
	- Command: ls -l ./challenges

19. (B) Append some text to the end of "restricted.txt". It's OK to do this in
    2 steps.
	- Commmand: 
		- 1 - chmod 600 restricted.txt ("concede permissão de escrita")
		- 2 - echo "texto teste" >> restricted.txt

20. (B) Run the "hello_executable" program.
	- Command: ./hello_executable

21. (B) Run the "challenge_20" program. It's OK to do this in 2 steps.
	- command:
		- 1 - chmod 700 challenge_20 (apos verificar permissões)
		- 2 - ./challenge_20 (executa)

22. (B) Compile and run "compile_me.c". It's OK to do this in 2 steps.
	- Command: 
		- Install gcc (sudo apt install gcc)
		- gcc compile_me.c

23. (A) Run the "redirect" program and collect all of its output in a file
    named "output.txt".
	- Command: ./redirect > output.txt 2>&1

24. (B) Get the current date and time.
	- Command: data

25. (B) Show all of the running processes on your computer.
	- Command: top

26. (B) Show the number of processors/cores in your computer.
	- Command: nproc

27. (B) Find out what version of the Linux kernel is currently running.
	- Command: uname -r

28. (B) Find the file in the "bunch_of_files/" directory that contains the string:
    "You found the needle in the haystack!"
	- Command: grep -r "You found the needle in the haystack!"

29. (B) Print the first 25 lines of people.csv.
	- Command: head -n 25 people.csv

30. (B) Print the last 25 lines of people.csv.
	- Command: tail -n 25 people.csv
31. (I) Display just the differences between greeting1.txt and greeting2.txt
	- Command: diff greeting1.txt greeting2.txt

32. (I) Print "Hello", then wait 5 seconds, then print "world!".
	- Command: echo "Hello" && sleep 5 && echo "World"

33. (I) Create a 1MB file full of zeros.
	- Command: dd if=/dev/zero bs=1024 count=1024  | tr '\0' '0' > file_zeros

34. (I) Create a 2MB file full of random data.
	- Command: dd if=/dev/urandom of=random_file bs=2048 count=1000

35. (I) Count the number of lines in README.txt.
	- Command: wc -l README.txt

36. (B) Display the contents of README.txt in reverse (last line first).
	- Command: tac README.txt

37. (I) Display all of the last names in people.csv.
	- Command: head people.csv | cut -d , -f 2

38. (A) Count the number of unique last names in people.csv.
	- Command: cut -d , -f 2 people.csv | sort | uniq | wc -l

39. (A) Did you accidentally count the CSV header in the previous challenge?

40. (A) There's a second way to exclude the CSV header from your count. Find it.

41. (A) Now that you've found two ways to correctly count the number of unique
    last names in people.csv, can you prove whether or not one is more efficient
    (faster) than the other?

42. (A) Count the number of people with the first name "Josiah" in people.csv.

43. (I) Count the number of files (not directories) in the "challenges" directory .

44. (I) Count the number of subdirectories in the "challenges" directory.

45. (I) Remove all files with "deleteme" in the name.

46. (I) In challenge 28 you found a file. Replace the string "You found the
    needle in the haystack!" with "The needle has been removed."

47. (A) Transform people.csv from ',' delimited to '|' delimited and save the result in people_pipe.csv.

48. (A) Find all of the files in "bunch_of_files/" that are duplicates of "file001.rand".

49. (A) Execute this challenge in exactly 2 steps

    1) (B) Create an empty file named "supercalifragilisticexpialidocious.txt".
    2) (A) Remove "supercalifragilisticexpialidocious.txt". Your command may
           only use a maximum 5 total characters (no wildcards or globs).

50. (A) Create a set of empty files. Each file has a name in the form "L-N.txt"
    where L is a letter and N is a number. Valid letters are a,b,c, while valid
    numbers are 1,2,3. Create all permutations (total of 9 files). Make your
    command as short as possible. I can do it in 25 characters, can you do
    better?

BONUS: Create a challenge of your own and ask a friend to complete it.

Congratulations! You've completed all of the challenges. If you haven't
already, go back through and find different ways to do some of the challenges.
Compare notes with a friend!
