# Way of working

In this document you will find most information on the way of working for engineers at In2Event.
This will, in general, be how most engineering team will work.

> **Note**
> We are constantly improving our way of working. So, this document will and can change frequently.

The WOW can be divided into two part: planning and developing.

## Planning

### 1. Writing issues

Before we can actually start planning we need to write down what we are going to work on.
We do that in Github issues per repository. Each issue contains a small descriptions on what the goal is of the issue
and then some additional information, like a design file for example, if that is available.

Also, there should be a list called acceptance criteria. This checklist describes when the issue is done.

### 2. Planning the work

We are working in cycles of 2 weeks. Every two weeks we plan for the next two weeks.
During this meeting we look at the previous two weeks and reflect on what was done and what needed more time.

Together we determine how much work we can do for the following two weeks. We keep track of this on a [Github board](https://github.com/orgs/In2Event/projects/6/views/2)

## Developing

### 1. Creating a branch

The naming of the branch should be as following: `feature/{issue number}`. The reason for this is that other people can easily find the branch related to an issue. You can create a branch in the interface of github when you have an issue open, use the command line of git or a visual git application.

### 2. Draft pull request

When you start developing it's always a good idea to do commits and push them to the remote branch. If something would happen to your laptop or you are sick other people can pick up the work where you left it. Github gives the ability to create draft pull request. This is a good indication for other engineers that you are still working on it and that it is not ready to be reviewed. Also, the pipelines are designed not to run when a pull request is in draft.

By creating a draft pull request you can check the request yourself and improve it before asking other people for a review.

### 3. From draft to non draft

When you are done with the issue, the code meets all the acceptance criteria and the pull request looks good you can convert it to a non draft pull request.
Now the pipeline will run and some checks. It will also deploy your code to a test environment.

### 4. Review

Before you can merge the pull request you must always ask for a review from an other engineer. This ensures code quality and helps people learn from each other.

## Definition of done

- New code has unit tests
- Unit tests passed
- Manual tests passed
- Acceptance criteria met
- Pipeline is green
- Code reviewed