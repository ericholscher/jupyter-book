---
substitutions:
    ReadTheDocs: "[ReadTheDocs](https://readthedocs.org)"
---
# ReadTheDocs

{{ReadTheDocs}} is a web service for hosting documentation online.
They offer free web hosting for open source projects, sustained by [ethical advertising](https://docs.readthedocs.io/en/stable/advertising/ethical-advertising.html) that is inserted into pages.

{{ReadTheDocs}} builds Sphinx websites, and does not support Jupyter Book directly.
However, you can [convert your book to a Sphinx website](../sphinx/index.md) in order to publish with {{ReadTheDocs}}.

To publish your book with {{ReadTheDocs}}, follow these steps:

1. **Get started with ReadTheDocs**.
   To do so, follow [the ReadTheDocs tutorial](https://docs.readthedocs.io/en/stable/tutorial/index.html).
   Configure {{ReadTheDocs}} to host a website from your book's repository.
2. **Convert your book into a Sphinx site**.
   There are two ways to do this using the Jupyter Book CLI.

   - [Manually convert your book to a Sphinx site](sphinx:convert).
   - [Use `pre-commit` to automatically convert your book to sphinx](sphinx:convert:pre-commit).

   In either case, it will generate a `conf.py` file along with your book's source files.
   This is the file Sphinx uses to build your book.
3. **Commit the `conf.py` file and push to your online repository**.

If you've configured {{ReadTheDocs}} correctly, it should now automatically build your book's HTML and host it online.
