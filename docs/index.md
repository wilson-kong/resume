# Welcome ☺
This website is dedicated to outlining my experience and skillsets.
<!-- For full documentation visit [mkdocs.org](https://www.mkdocs.org). -->

<!-- ## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit. -->

- [Welcome ☺](#welcome-)
  - [Education](#education)
  - [Work experience](#work-experience)
    - [Software Industry Mentor - Python(Django, DRF)](#software-industry-mentor---pythondjango-drf)
    - [Software Engineer - Teaching Assistant](#software-engineer---teaching-assistant)
  - [Projects](#projects)
  - [Volunteer experience](#volunteer-experience)

## Education
| Bachelor of Engineering (Honours) and Master of Engineering |  The University of Queensland |
| :---------------- | ----: |
| Majoring in Mechatronics ||

--------------------------------------------------
## Work experience
=== "Python"
    ```python title="work_class.py"
    class Work: # Click me -> (1) <-
        def __init__(self, title: str, company: str, duration: tuple, location: str):
            """ Creates an instance of work.
                Parameters:
                    title: Job title.
                    company: Company name.
                    duration: start and end dates of the role. i.e. (start, end)
                    location: Location of job
            """
            self._title = title
            self._company = company
            self._start = duration[0]
            self._end = duration[1]
            self._location = location
            self._responsibilities = []

        def add_responsibility(self, responsibility: str):
            """ Add a responsibility to this role.
                Parameters:
                    responsibility: description of responsibility.
            """
            self._responsibilities.append(responsibility)

        def __str__(self) -> str:
            """ Return the role description """
            output = f'Work as a {self._title} at {self._company} '
            output += f'located in {self._location} '
            output += f'from {self._start} to {self._end}.'

            if self._responsibilities:
                output += '\nMy key responsibilities include:\n'
                
                for responsibility in self._responsibilities:
                    output += f'- {responsibility}\n'

            return output
    ```

    1. Feel free to copy this code to your computer 💻 to set up the work class.

=== "Java"
    ```java title="WorkClass.java"
    import java.util.ArrayList;
    import java.util.List;

    class Work {
        private String title;
        private String company;
        private int start;
        private int end;
        private String location;
        private List<String> responsibilities;

        public Work(String title, String company, int start, int end, String location) {
            /** Creates an instance of work.
            * @param title: The title of the job.
            * @param company: The company that the job is at.
            * @param start: The year that the job started.
            * @param end: The year that the job ended.
            * @param location: The location of the job.
            */
            this.title = title;
            this.company = company;
            this.start = start;
            this.end = end;
            this.location = location;
            this.responsibilities = new ArrayList<>();
        }

        public void addResponsibility(String responsibility) {
            /** Adds a responsibility to the role.
            * @param responsibility: The responsibility to add.
            */
            this.responsibilities.add(responsibility);
        }

        @Override
        public String toString() {
            /** @return: A string representation of the work. */
            String output = "Work as a " + this.title + " at " + this.company + " ";
            output += "located in " + this.location + " ";
            
            if (this.end == 2023) {
                output += "from " + this.start + " to present.";
            } else {
                output += "from " + this.start + " to " + this.end + ".";
            }
            
            if (!this.responsibilities.isEmpty()) {
                output += "\nMy key responsibilities include:\n";
                for (String responsibility : this.responsibilities) {
                    output += "- " + responsibility + "\n";
                }
            }
            return output;
        }
    }
    ```

### Software Industry Mentor - Python(Django, DRF)
=== "Python"
    ```python title="Python shell"
    >>> duration = (2023, 'present')
    >>> work = Work(
            'Software Industry Mentor - Python(Django, DRF)',
            'She Codes',
            duration,
            'Brisbane or Meeanjin'
        )
    >>> work.add_responsibility('Python education. Object-oriented programming '\
        'philosophies and best practices.')
    >>> work.add_responsibility('Providing practical learning opportunities '\
        '(Python, Django, DRF (Django Rest Framework) with React front end)')
    >>> work.add_responsibility('Teaching adult students to create a '\
        'DRF backend and SQL light db, deploying to fly.io. '\
        'CI/CD pipeline with Github Actions. ')
    >>> work.add_responsibility('Automated-test development for projects. ')
    >>> work.add_responsibility('Working alongside other mentors and software '\ 
        'engineers.')
    >>> print(work)
    ```

=== "Java"
    ```java title="Main.java"
    public class Main {
        public static void main(String[] args) {
            int startYear = 2023;
            int endYear = 2023;
            
            Work work = new Work(
                "Software Industry Mentor - Python(Django, DRF)",
                    "She Codes",
                    startYear,
                    endYear,
                    "Brisbane or Meeanjin"
            );
            work.addResponsibility("Python education. Object-oriented programming " +
                    "philosophies and best practices.");
            work.addResponsibility("Providing practical learning opportunities " +
                "(Python, Django, DRF (Django Rest Framework) with React front end)");
            work.addResponsibility("Teaching adult students to create a " +
                "DRF backend and SQL light db, deploying to fly.io. " +
                "CI/CD pipeline with Github Actions.");
            work.addResponsibility("Automated-test development for projects. ");
            work.addResponsibility("Working alongside other mentors and software " +
                "engineers.");
            System.out.println(work);
        }
    }
    ```

### Software Engineer - Teaching Assistant
=== "Python"
    ```python title="Python shell"
    >>> duration = (2019, 'present')
    >>> work = Work(
            'Software engineer - Teaching assistant',
            'The University of Queensland',
            duration,
            'Brisbane or Meeanjin'
        )
    >>> work.add_responsibility('Designing and developing software learning'\ 
    'resources and assessment pieces.')
    >>> work.add_responsibility('Python unit testing, static analysing, and '\
    'grading tool integration (Gradescope) for a number of major assessments'\ 
    'since 2021.')
    >>> work.add_responsibility('Providing training for new tutors.')
    >>> work.add_responsibility('Stakeholder engagement with the uni to plan'\ 
    'and decide the direction of courses and a student\’s university career.')
    >>> work.add_responsibility('Regularly reporting to the course-coordinator.')
    >>> work.add_responsibility('Teaching coding concepts in Python, C++ '\
    '(Arduino), Java, and C.')
    >>> print(work)
    ```

=== "Java"
    ```java title="Main.java"
    public class Main {
        public static void main(String[] args) {
            int startYear = 2019;
            String endYear = 2023;
            Work work = new Work(
                    "Software engineer - Teaching assistant",
                    "The University of Queensland",
                    startYear,
                    endYear,
                    "Brisbane or Meeanjin"
            );
            work.addResponsibility("Designing and developing software learning" +
                "resources and assessment pieces.");
            work.addResponsibility("Python unit testing, static analysing, and " +
                "grading tool integration (Gradescope) for a number of major assessments since 2021.");
            work.addResponsibility("Providing training for new tutors.");
            work.addResponsibility("Stakeholder engagement with the uni to plan" +
                "and decide the direction of courses and a student\’s university career.");
            work.addResponsibility("Regularly reporting to the course-coordinator.");
            work.addResponsibility("Teaching coding concepts in Python, C++ " +
                "(Arduino), Java, and C.");
            System.out.println(work);
        }
    }
    ```

--------------------------------------------------
## Projects
* [Wordle Clone](https://wilson-kong.github.io/games)

--------------------------------------------------
## Volunteer experience

<!-- ## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files. -->

