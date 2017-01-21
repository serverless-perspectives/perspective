# Purpose

To facilitate collaboration on a Serverless Perspective whitepaper/research document. 

    "Rigorous citation paired with wild speculation."

# Getting Started

1. Install Docker

1. Download and install [BibDesk](https://sourceforge.net/projects/bibdesk/) - you'll use it to save sources

1. Start writing. We'll add some thoughts to 'example.md' first.
 
1. Add your first citation. Open 'sources.bib' in BibDesk and use the handy UI to enter your source, ensuring that create a unique 'Cite Key'. If you are feeling brave, you can edit sources.bib in a text editor instead!

1. In your markdown file, in this case, 'example.md', reference the cite key in your text. In this case, we've referenced [@amazon-eating] after the first sentence.

1. All done? That was fast. Go ahead a create a beautifully formatted pdf. Replace the first part of the '-v' command with the directory where you cloned this repository:

    ``` 
    docker run --rm -v ~/src/perspective:/source jackwarner/serverless-perspectives example.md --smart --standalone --bibliography sources.bib --csl=/styles/chicago-fullnote-bibliography.csl -o example.pdf
    ```

1. Or epub:

     ``` 
     docker run --rm -v ~/src/perspective:/source jackwarner/serverless-perspectives example.md --smart --standalone --bibliography sources.bib --csl=/styles/chicago-fullnote-bibliography.csl -o example.epub
     ```

1. Don't love Chicago Fullnote Bibliography? Just head over to [https://github.com/citation-style-language/styles](https://github.com/citation-style-language/styles) and find a format that's more your 'style'. Re-run the command with the new style:

    ```
    docker run --rm -v ~/src/perspective:/source jackwarner/serverless-perspectives example.md --smart --standalone --bibliography sources.bib --csl=/styles/american-journal-of-climate-change.csl -o example-climate-change.pdf
    ```

# Works Cited

The approach for generating beautifully formatted 