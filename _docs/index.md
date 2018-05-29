---
title: Getting Started
permalink: /docs/index/
---

## About the Data

If you are interested exploring the data immediately, use left hand bar to navigate to the different datasets we have created for the different libraries listed. 

If you are interested in our methodology for creating the data, please read below:

1. **Create a List of Books that have Hebraic Content** - Dr. Arthur Kiron of the University of Pennsylvania Libraries first physically went to the libraries themselves a, examining them for Hebraic content. 
2. **Accessing the catalogues** - Once we had an idea of the authors and titles that would have Hebraic content in a colonial library we began using online tools, like Google Books and Hathi Trust to access the catalogues of the various libraries of Colonial America. 
3. **Marking the Catalogue** you have the catalogues, mark down which books correspond to the corpus list from step 1. (We often would simultaneously do this with step 5)
4. **List feature in WorldCat** - Create a list in a WorldCat Using these catalogues we created an account in WorldCat and used the list feature they offer. We created a seperate list for each catalogue we evaluated.
5. **Add the appropriate edition to the list** - We would look at WorldCat looking at whichever catalogue entry corresponded to the matching list entry from step 3 and we would add them to our "list" in WorldCat. The crucial part about this step was that on WorldCat you cannot just search for the title in the searchbox and assume that title corresponds to the title looking for because they happen to match.  There can be different editions for one book (you can see this if you filter by year) and even within one year there can be many different editions or entries for that one book depending on how a library chose to enter the metadata ( meaning the author, title, publication place etc.). Because of this, it is important to think carefully about which edition you decide you add to your list. 
6. **Export your list** - Once you are done going through a catalogue you can export it to a spreasheet. WorldCat has the ability to export each list to a CSV. *Make sure you do not open a CSV with Hebrew or Arabic characters in Excel, it will corrupt the file. Only open the CSV on Google Sheets or Open Refine.* 

## Writing content

### Docs

Docs are [collections](https://jekyllrb.com/docs/collections/) of pages stored under `_docs` folder. To create a new page:

**1.** Create a new Markdown as `_docs/my-page.md` and write [front matter](https://jekyllrb.com/docs/frontmatter/) & content such as:

```
---
title: My Page
permalink: /docs/my-page/
---

Hello World!
```

**2.** Add the pagename to `_data/docs.yml` file in order to list in docs navigation panel:

```
- title: My Group Title
  docs:
  - my-page
```

### Blog posts

Add a new Markdown file such as `2017-05-09-my-post.md` and write the content similar to other post examples.

### Pages

The homepage is located under `index.html` file. You can change the content or design completely different welcome page for your taste. (You can use [bootstrap components](http://getbootstrap.com/components/))

In order to add a new page, create a new `.html` or `.md` (markdown) file under root directory and link it in `_includes/topnav.html`.
