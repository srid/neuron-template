---
tags: [other]
---

# FAQ

How long does it take for the site to update?
:  The [GitHub Actions](https://github.com/features/actions) build itself takes about ~15 seconds to run. It is generally expected for your site to update around that duration, and take no more than a minute.

Which environment is used to build and deploy the site?
: From the [Actions workflow file](https://github.com/srid/neuron-template/blob/master/.github/workflows/publish.yaml), it can be seen that we use the [official neuron docker image](https://neuron.zettel.page/docker.html), as well as use the  [peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages) action to push the built site to the `gh-pages` branch, that in turn gets deployed to GitHub's servers.

How can I use the stable version of neuron?
: The Actions workflow file `publish.yml` is configured to pull the *latest* docker image; you can adjust it to pull from a (unchanging) tag instead. [See here][docker-tags] for a list of available tags which correspond to neuron versions; generally you would pick the latest tag and put it in `publish.yml`. Then, your site will continue use the same neuron version, regardless of upstream development changes.

Can I use my own domain name?
: Yes, you can [set the CNAME in publish.yaml][cname].

How can private repositories be published?
: You will need a GitHub paid plan to publish private repositories. Public repositories on the other hand can be published in the GitHub free plan. [Cerveau](https://www.cerveau.app/)'s Premium Plan, when it is ready, will be able to publish public and private repositories.

[cname]: https://github.com/peaceiris/actions-gh-pages#%EF%B8%8F-add-cname-file-cname
[docker-tags]: https://hub.docker.com/r/sridca/neuron/tags?page=1&ordering=last_updated
