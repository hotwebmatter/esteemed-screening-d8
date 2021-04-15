# esteemed-screening-d8

As the Esteemed Screening Department scales to accommodate more candidates, we
expect to receive a lot of Drupal 8 and Drupal 9 code examples for review.

This repository uses Acquia BLT to provide a convenient method for rapidly
evaluating code samples for adherence to Drupal coding standards.

Each candidate's code sample will also be saved in the repository as a feature
branch, in case a client asks to see a sample of a candidate's work.

Documentation forthcoming on the screening process, but in a nutshell:

* Clone this repository to your local workstation.

```
$ git clone git@github.com:hotwebmatter/esteemed-screening-d8.git
```

* Create a new git branch for the candidate's code sample:

```
$ git checkout -b candidate_name
```

* Save their code in the appropriate location for custom module or theme.

* Use BLT to run tests on their code. [README-BLT](./README-BLT.md)

* Forthcoming: local dev preview, possible deploy to screening environment.
