# We're Use Git!

And we'll be using it more and more.

## Git Repository Hosting

We currently use 3 git repository hosting environments:

1. [On-premise GitLab](https://gitlab.grad.arizona.edu/) (omnibus edition), which houses the bulk of our versioned code and handles most CI/CD actions that we employ. Our GitLab instance is only accessible from within the Graduate College MPLS bucket and VLANs.
2. [Graduate College Bitbucket](https://bitbucket.org/uazgraduatecollege), which we use primarily to host code that we share with other University developers.
3. [Graduate College GitHub](https://github.com/uazgraduatecollege), which we are only just beginning to use.

While we anticipate continuing use of and expansion into Bitbucket and GitHub for certain use cases, GitLab will continue to be our primary Git hosting platform for the foreseeable future.

## Preferred Workflows

For most projects we use a [Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow), ie. fork, branch, merge. This is the preferred workflow for everything but our Drupal assets.

For Drupal, we more typically use either a [Centralized Workflow]() (primarily when updating Drupal core or 3rd-party module references in our [Drupal Platforms](https://gitlab.grad.arizona.edu/drupal/uagc_drupal/)) or a [Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow), ie. branch & merge, which we're more likely to employ when updating Graduate College modules, features, or themes.

Further References: Atlassian article [Comparing Git Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows).

## Code Versioning

By design, Git is the tool we use to [version all code](best-practices/version-all-code.md).

## Continuous Integration and Continuous Delivery

(To do)
