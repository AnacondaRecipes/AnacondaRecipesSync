# AnacondaRecipesSync
Repo of submodules for organizing and executing sync with AnacondaRecipes

This is intended to be a temporary aggregation of recipes to facilitate the merge of AnacondaRecipes with their conda-forge parent recipes.  These recipes were created by:

1. Forking conda-forge to AnacondaRecipes
2. editing recipe to use new CB3 features (especially the variant pinning, run_exports and compiler jinja2)
3. rebase changed recipes on current conda-forge recipe.  Resolve merge conflicts.
4. push to branch

In theory, the branch in step 4 should be mergeable with conda-forge with no conflicts.  These recipes are being tested, but may not work right off the bat in their current state, if there were mistakes made in resolving merge conflicts.

The next step is to test building each of these recipes. If they pass, they can be merged into AnacondaRecipes master branch.  That branch should then replace or create a cf-sync branch in the AnacondaRecipes repo.  A PR should then be issued from that cf-sync branch to the parent conda-forge feedstock.
