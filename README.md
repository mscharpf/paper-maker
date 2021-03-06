Build your paper with GitHub actions
====================================

This will use GitHub Actions to build your LaTeX manuscript and push the compiled PDF back to GitHub. It assumes that your manuscript is `paper/ms.tex`, but this can be changed by editing `MANUSCRIPT_PATH` in `action.yml`.

This is nothing new. [Dan Foreman-Mackey](https://github.com/dfm/) made it work with Travis CI first, but now since GitHub Actions are _new on the block_, I thought I'd try them out. They're pretty sweet!

Next step,... `latexdiff`...

Use it!
-------

This Action is [hosted on the Marketplace](https://github.com/marketplace/actions/paper-maker). If you want to use it you can just put the following snippet into your `.github/workflows/action.yml` file:

````
- name: paper-maker
  uses: andycasey/paper-maker@0.10
````

Or you can clone/fork/copy/fax the `action.yml` file in this repository and put it into your `.github/workflows/` folder in your repository. That's it! No extra permissions, no extra steps, no nothing!

**Now write the damn paper!**
