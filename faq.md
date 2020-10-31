---
tags: [other]
---

# FAQ

How long does it take for the site to update?
:  The [GitHub Actions](https://github.com/features/actions) build itself takes about ~25 seconds to run. It is generally expected for your site to update around that duration, and take no more than a minute.

Which environment is used to build and deploy the site?
: From the [Actions workflow file](https://github.com/srid/neuron-template/blob/master/.github/workflows/publish.yaml), it can be seen that we install [neuron](https://neuron.zettel.page/) using GitHub's artifact storage in Srid's repo [srid/neuron](https://github.com/srid/neuron), as well as use the  [peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages) action to push the built site to the `gh-pages` branch, that in turn gets deployed to GitHub's servers.

Can I use my own domain name?
: Yes, you can [set the CNAME in publish.yaml][cname].

How can private repositories be published?
: You will need a GitHub paid plan to publish private repositories. Public repositories on the other hand can be published in the GitHub free plan. [Cerveau](https://www.cerveau.app/)'s Premium Plan, when it is ready, will be able to publish public and private repositories.

[cname]: https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-add-cname-file-cname
