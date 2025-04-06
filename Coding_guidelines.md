# General Coding Guidelines 

> Follow a clear code structure:
  > Use meaningful variable names,and fumction names.(sum instead of s etc..)
  > Keep your code modular break down the code into small reusable functions.
  > keep the lines short (preferably under 80-100 charecters).
  > keep the number of lines limited within a function (preferably under 80-100 lines).
  > add blank lines between the sections to improve readability.

> Use Comments Wisely
  > Write meaningful comments but don't over do it.
  > Explain why not what (good code is self-explanatory).
  > Use inline comments only for complex logic. (eg: some complex pointer code might need example).
    > Example : 
              Bad Commenting:
                x=x+1;//This adds 1 to x (Its obvious and can be understood easily)
              Good Commenting:
                //Increse the counter to track the number of attempts 
                attempts+=1;
  > Try to use multi-lined comments to briefly describe the use of function instead.

> Follow Naming Conventions
  > acoording to language you use try to follow the name conventions.
    > snake_case : Rust, C,Python.
    > SCREAMING_SNAKE_CASE: Used for the constants (MAX_TIME).

> Bracing Style
  > Always use side braces {} for functions and control structures.
  > Avoid K&R style.
    > Example : Follow This :-
    int main() {
    if (condition) {
        // Do something
      }
    }
    >> Avoid using bottom braces like K&R style: 
      int main()
    {
       if (condition)
     {
        // Do something
     }
    }

> Avoid Hardcoding values 
  > Always use constants or configuration values.
    > Example :
        int maxSpeed=120; (PREFERABLY AVOID)
        final int MAX_SPEED=120; (GOOD PRACTICE!)

> Use Proper Error Handling :
 > Always handle your errors before your program crash.
   > Example: USing Result in Rust for safer error handling.
    
    use std::fs::File;

      fn open_file() -> std::io::Result<File> {
      File::open("data.txt") // This returns an error instead of panicking
    }

> Optimize Code Performance.
  > Avoid unnecessary computations and memory allocations.
  > Use loops efficiently (avoid nested loops if possible).
  > Use data structures wisely (choose HashMap over List when needed).
  > Sort data once instead of sorting multiple times inside loops.

> Always use Git for tracking changes in your code.
  > Write clear commit messages (Fixed login bug instead of Update).
  >Use present tense in commit messages
      Do this:
       Login: Add validation for empty fields
      Not this:
       Login: Added validation for empty fields
  > Use imperative mood (like giving a command), as if you're telling the code what to do. This keeps the history clean and consistent.
  > Use branches for new features (feature/user-authentication).

     git init
     git add .
     git commit -m "Initial commit"
     git push origin main 
       NOTE: As a contributor, you cannot directly make changes to the repository. Make sure to send PRs for any changes or contributions to the project.
  > Pull Request Guidelines
    > Always merge into the main branch:
        PRs should target the main branch. Avoid creating or merging into custom branches unless explicitly discussed.
    > Compare with main:
        When opening a pull request, make sure your branch is compared against main, not a newly created branch.
   > This ensures smoother merges, accurate change tracking, and a consistent workflow for everyone.


> Keep Learning & Improving
  > Read documentation.
  > Write tests to ensure your code works as expected.
  > Refactor your code to improve readability and efficiency.


Good coding practices save time, reduce bugs, and make teamwork easier. Follow these guidelines, and your code will be clean, efficient, and maintainable!

# Contribution Guidelines
 Hey there! First off, thank you for your interest in contributing to this project. We appreciate your time and effort! To keep things smooth and collaborative, here are a few simple guidelines to follow:
  > Fork & Branch Smartly
     >Always fork the repo before making changes.
     >Create a new branch for your work (e.g., feature/add-login, fix/ui-bug). This helps keep things organized. 

  > Before you send a Pull Request (PR):
     > Make sure your branch is up to date with main.
     > Test your changes to confirm everything works.
     > Write a short but clear PR description—tell us what you did and why!
     > If your PR fixes an issue, mention it like this: Fixes #123.

  > Write meaningful commit messages. 
     > Follow the project’s code style. If we have a linter or formatter, please use it!
     > If your changes impact functionality, update the docs too.
 
  > Feedback Helps Us Build Better !
     > Code reviews help us improve—don’t take feedback personally!
     > If maintainers request changes, try to address them quickly.
    
  > Be direct in the conversation with maintainers and do not be too formal or too informal get straight to point.
  > Be kind, patient, and respectful. We’re all here to learn and build something cool together.