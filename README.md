StanfordLinkPredictor-wikibot
=============================

This is a wikipedia bot which inserts links between wikipedia pages based on statistical inference of navigational traces

The job of this bot is to insert link between a source and a target page, given the mention in the source page which should link to the target page
The input is in the form of a tab separted file
<Source article>  <target article>  <mention>
To make this bot version agnostic, it provides a best effort service, wherein it searches for the mention in the source article. If the mention exists then the link is added (at the first mention) other-wise it is not.
It does not support specifiying location of the mention (in terms of number of words preceeding it) because it is subject to change due to edits. 

The link prediction algorithm is not a part of this bot.
