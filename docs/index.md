# Welcome to Wilson
This website is dedicated to outlining my experience and skillsets.
<!-- For full documentation visit [mkdocs.org](https://www.mkdocs.org). -->

<!-- ## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit. -->

- [Welcome to Wilson](#welcome-to-wilson)
  - [Education](#education)
  - [Work experience](#work-experience)
    - [Industry Mentor - Python(Django, DRF)](#industry-mentor---pythondjango-drf)
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
    ```python
    class Work:
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

=== "Java"
    ```java
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

### Industry Mentor - Python(Django, DRF)
=== "Python"
    ```python
    >>> duration = (2023, 'present')
    >>> work = Work(
            'Industry Mentor - Python(Django, DRF)',
            'She Codes',
            duration,
            'Brisbane or Meeanjin'
        )
    >>> work.add_responsibility('Python education. Object-oriented programming '\
        'philosophies and best practices.')
    >>> work.add_responsibility('Django, DRF, and React mentoring.')
    >>> work.add_responsibility('Communicate and mentor adults that have spent '\
        'time in different fields.')
    >>> print(work)
    ```

=== "Java"
    ```java
    public class Main {
        public static void main(String[] args) {
            int startYear = 2023;
            int endYear = 2023;
            
            Work work = new Work(
                "Industry Mentor - Python(Django, DRF)",
                    "She Codes",
                    startYear,
                    endYear,
                    "Brisbane or Meeanjin"
            );
            work.addResponsibility("Python education. Object-oriented programming " +
                    "philosophies and best practices.");
            work.addResponsibility("Django, DRF, and React mentoring.");
            work.addResponsibility("Communicate and mentor adults that have spent " +
                    "time in different fields.");
            System.out.println(work);
        }
    }
    ```

### Software Engineer - Teaching Assistant
=== "Python"
    ```python
    >>> duration = (2019, 'present')
    >>> work = Work(
            'Software engineer - Teaching assistant',
            'The University of Queensland',
            duration,
            'Brisbane or Meeanjin'
        )
    >>> print(work)
    ```

=== "Java"
    ```java
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

