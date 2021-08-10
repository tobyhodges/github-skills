# Repository Metadata

Make your repositories more findable and accessible by annotating them with
some basic information.

1. Go to a repository that you have _Maintain_ or _Admin_ access to
   e.g. any personal repository.
2. Click the gear/cog :gear: symbol near the top right of the repository window,
   next to _About_.
3. Here you can
  4. write/edit the repository description: a title or very short summary of the project.
  5. add a URL for the website associated with the repository.
     If there is a GitHub Pages site built from this repository,
     go to _Settings_ -> _Pages_ and copy the URL from there, before pasting it into
     the _Website_ field of this _Edit repository details_ box.
  6. add _Topics_: keywords that help people find your repository when searching
     for particular kinds of projects on GitHub.

As well as helping your repository be more findable via GitHub's search,
repository metadata can be used by other applications to fins/list your project.
For example, in The Carpentries,
our [Community Developed Lessons page](https://carpentries.org/community-lessons/)
uses the GitHub API to build a table of all repositories in The Carpentries Incubator and Lab
that have the `lesson` topic.
That table includes:

- the repository _description_ as the lesson title.
- the [lesson life cycle stage](https://cdh.carpentries.org/the-lesson-life-cycle.html#overview-and-definitions)
  based on the presence of a `pre-alpha`/`alpha`/`beta`/`stable` topic.
- the other topics as tags on the lesson, to help people filter the table
  and more easily find a lesson they want to teach/read/contribute to.
