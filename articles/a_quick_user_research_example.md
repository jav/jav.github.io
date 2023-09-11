# [](#header-1) A quick user-research example
### An example of a quick user-feedback scenario.
###### 2023-09-11

Today, with my team of developers at IKEA, we got into a discussion on the appropriate scope of a story.

The contention was between 
1. Doing as little as necessary before putting working software infront of users ([Yagni](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it))
2. Extending scope with input field validation and auto-completion features that we thought are highly-likely to enhance the user experience and prevent future extra work.

Another perspective is "What's the right balance between effort and speculative future benefit".

We finally landed in the conclusion to remove the input-field auto-completion features.

The thought didn't leave me, and I ended up doing two quick users tests.

The input fields where (a little simplified):
* What is our Global Catalog System name?
* What is our Cost-center?
* What is our Project code?
* What is our Azure group?

My hypothesis is that people will look these up and copy-paste. Meaning that mistyping will be unusual.

**Interview 1**

I reached out to a manager colleague, asked them to use the feature, and to find the data necessary.

Through that interview I discovered that:
* mistyping will still be common.
* Formats vary for cost-center or project code
  * E.g. cost center can be any of `1234`, `CC1234`, `CC_1234`
* It's not obvious that Azure group and 'AD group' are the same, nor how to find your own group.
* Once you're through the input-field validation that already exists
  * Getting an error on the nextpage and clicking `< Back`, will take you to the original form, with empty fields.



**Interview 2**

I hypothesize that our main users will be other developers.

So I asked all members of our own team:
> Please find the following information and message it and roughly how long it took you to find it to me privately.
>
> * What is our Global Catalog System name?
> * What is our Cost-center?
> * What is our Project code?
> * What is our Azure group?

I want to compare the time it takes to find the information, and also how many different formats I get it in.

I'm still waiting for the results, but the few that I have received  so far suggest that:
* The information is fast to find 
* Inputted format varies

> ∴
> 
> It's likely that input validation is going to stop a lot errors
>
> It is less likely that autocompletion is an important feature


