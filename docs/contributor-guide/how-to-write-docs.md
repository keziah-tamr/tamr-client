# How to write docs

Before you begin to add content, decide which of the three types of content you want to add:
1. Tutorial
2. How-To guide
3. Explanation

``` note::
    There is fourth type of content, known as Reference.

    For the Tamr Client, you don't need to add reference topics manually because reference documentation for the Tamr Client is generated automatically based on the source code.

    For more details, see Reference description below.
```

For more information about each type of content, see the following descriptions.
Also see [Divio's documentation system manual](https://documentation.divio.com/).

### Tutorial

Tutorials are learning-oriented and ...

- Must include an end-to-end walkthrough for a specific use case, such as "Tutorial: Deduplicating buildings in Cambridge".
- Must have a clearly stated goal and allow the users to achieve it after they complete the steps in the tutorial.
- Must provide the sample data and input configuration that are necessary for the user to complete the tutorial. Include this information upfront, at the start of your tutorial.
- Must be self-contained, but can include links to procedures described elsewhere in this documentation.

Tutorials are useful if the use case is both simple and in high demand.
Not every use case deserves a tutorial.
Before writing a tutorial, think first of a use case that has a high learning value, and then prepare the assets needed to complete your tutorial, such as a sample dataset and sample configuration.

Tutorials are in high demand.
If you write a good one, many users will reference it and thank you for your work!

### How-To

How-Tos are task-oriented and ...

- Must include a list of numbered steps, known as a task, or a procedure, to help users complete a specific, domain-agnostic task, such as running a request, copying a file, installing, exporting, or other. For example, you can create a task titled "How to stream datasets out of Tamr".
- Must include a context paragraph, such as "It is often useful to stream datasets from Tamr, to load them into business analytics applications, such as Tableau, for analysis." Context may also include checks needed to be in place before users start the task, and links to related concepts. Context must provide information needed to begin the task, such as, it can list the host and port URL at which the endpoint for the service is served.
- Must include a stem sentence, such as: "To stream a dataset out of Tamr:" The stem sentence is followed by numbered steps.
- Must include a numbered list of steps where each step must begin with an imperative verb, such as: "Run the following curl request.", or "Save the file". For more examples see [Use Imperatives in Procedures](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/cmt-40/kantoo/vol40/doc/kce/styleguide/imperatives.html).

### Explanation

Explanations are understanding-oriented and ...

- Must explain a single concept of the Tamr Python client. If you'd like to write another concept, create it separately.
- Must [keep sentences short](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/cmt-40/kantoo/vol40/doc/kce/styleguide/shortsentences.html).
- May include examples of code or text examples.

### Reference

Reference is information-oriented.

It is something that users cannot remember and want to be able to refer to, often.
Reference provides details, such as configuration parameters for a particular method or call.
It never contains tasks, or concepts.
Reference is often automatically-generated from code, to ensure it is up-to-date and accurate at all times.

``` note::
    Our reference documentation is automatically generated by [autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html) based on type annotations and docstrings in the source code.
```