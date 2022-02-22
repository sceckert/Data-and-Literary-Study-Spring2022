# Research Exercise #5: Syllabi as Data

Feb 23, 2022

In this research exercise, we're going to look at three different datasets of syllabus data, as a way of asking what a syllabus (or many syllabi) can tell us about literary history.

There are three parts to this exercise. The bulk of the exercise is in Part 1 (which concludes with a short reflection) and Part 2 (which includes a few short questions for reflection.


## 1. *The Souls of Black Folks* in the Open Syllabus Project

The Open Syllabus Project (OSP), a non-profit founded that originated in the American Assembly (a Columbia University-affiliated think tank), is a database of just over 9 million college course syllabi and 7.2 million currently searchable metadata from those syllabi). 

In this next exercise, we're going to use the Open Syllabus Project's database to explore patterns in what texts are assigned in syllabiBecause of copyright reasons, the full text of syllabi are protected and not available fore download, nor are the metrics

+ 1.a Read the about page for the project, and browse through the ["Architecture + models" behind the project data](https://docs.opensyllabus.org/models.html). Don't panic if there are some technical terms––try to read with an eye towards understanding how the dataset was constructed, out of what materials, and what questions you might have about their methods. 
	+ Thing about what you've just read: what do we know (and not know) about the contents, scope, or origins of this dataset? 
	+ What things might we need to keep in mind if we wanted to make claims with this dataset? 

Let's explore the dataset! 

+ 1b. Using the [Open Syllabus Project's Explorer viewer](https://opensyllabus.org/), search the ["Titles" portal](https://opensyllabus.org/results-list/titles?size=50) for *The Souls of Black Folk* 
	+ What did you find? Did anything surprise you?
	+ Using the ["Titles" portal](https://opensyllabus.org/results-list/titles?size=50), search for both The Souls of Black Folk and Princeton
+ 1c. Using the ["Schools" portal](https://opensyllabus.org/results-list/schools?size=50), search a look at the syllabi specific to Princeton. 
	+ Are there patterns you notice?
+ 1d. Open the [Open Syllabus Project's Galaxy viewer](https://galaxy.opensyllabus.org/),
	+ Take a minute to read through [David McClure's post about the data behind this visualization](https://blog.opensyllabus.org/galaxy-v2/)
	+  Now, using the Galaxy viewer, search for *The Souls of Black Folk* , using both the "Search Books" and "Search Syllabi" functions. Jot down some notes about your findings
+ 1e.  Choose another text (or term––maybe a field or a genre) to search for. Jot down your findings
+ 1f.Take a quick peak at the beta-model ["Link Lab" view](https://blog.opensyllabus.org/link-lab/)
+ 1.g Finally, take a minute to write a quick reflection based on what you've found.




## 2. Columbia University's Literature Humanities Syllabus, 1937-2020

What if we wanted to look at a the syllabus history of a single literature course? What kind of questions could we ask?

Like Princeton's "Interdisciplinary Approaches to Western Culture" courses in the HUM sequence, Columbia has a core sequence of courses in Western literature and philosophy, dating back to the founding of university's great books curriculum during the interwar period (1919-1947). While we don't have an easily accessible set of material's on Princeton's core humanities sequence, we do have access to one version of Columbia's Core Curriculum records.

Take a look at the [Literature Humanities Texts 1937-2020 data](https://www.college.columbia.edu/core/1937.php) as described on the Literature Humanities website (also available in [this CSV](https://github.com/sceckert/Data-and-Literary-Study-Spring2022/blob/main/_datasets/Columbia-Literature-Humanities-Syllabi/columbia-university-literature-humanities-syllabus-texts-1937-2020.csv)). Download the [zip file containing the datasets](https://github.com/sceckert/Data-and-Literary-Study-Spring2022/blob/main/_datasets/Columbia-Literature-Humanities-Syllabi.zip?raw=true) Then, take a look at the the modified, more machine-readable version of the data I've collected in [this CSV](https://github.com/sceckert/Data-and-Literary-Study-Spring2022/blob/main/_datasets/Columbia-Literature-Humanities-Syllabi/columbia-university-literature-humanities-syllabus-texts-1937-2020-cleaned.csv), which omits Milton's *Lycidas* and standardizes the dates. Feel free to practice your Python skills and open up the modified CSV in a Jupyter notebook!  Think about what you might want to do to visualize this data.

Finally, take a quick peak at [this zip file of PDF excerpts from sample syllabi](https://github.com/sceckert/Data-and-Literary-Study-Spring2022/blob/main/_datasets/Columbia-Literature-Humanities-Syllabi/sample-literature-humanities-syllabi.zip?raw=true). (Note: these are just a very small representative sample of the kinds of syllabi that the dataset is drawn from)


+ 2a. What patterns do you notice?
+ 2b. What questions could we ask about this data? What might be some potential limitations to the data?



## 3. Finding Princeton archival syllabi

What if we wanted to find syllabi closer to home, in Princeton's literature departments?

In a few class sessions, we'll be heading to Special Collections in Firestone Library. We're going to warm up by practicing looking for course materials. 

+ Look through the finding aids to held in Firestone Library Special Collections Manuscript Division: [https://findingaids.princeton.edu/?f%5Brepository_sim%5D%5B%5D=Manuscripts+Division&group=true&q=syllabi&search_field=all_fields](https://findingaids.princeton.edu/?f%5Brepository_sim%5D%5B%5D=Manuscripts+Division&group=true&q=syllabi&search_field=all_fields)
+ Search for materials: I've put in "syllabi," but you could also try "course materials" or "reading list(s)" 
+ Once you've found something, navigate to one of the finding aids and, within the finding aid, to the particular set of material that your search.
+ Pick 2 or 3 items that you would want to potentially examine-- record the box or folder information, the collection and any other relevant collection call number.

Note: I've restricted the search to just the Manuscripts Division, since that's where we'll be visiting. But the University Archives. What if we [include Princeton University Archives (housed at the Mudd Library) in our search](https://findingaids.princeton.edu/?group=true&q=syllabi&search_field=all_fields)-- does anything cats your eye? 

Make note of any potentially interesting material!