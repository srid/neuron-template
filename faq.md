# FAQ

Why does the site not update *instantly*?
:  The [GitHub Actions](https://github.com/features/actions) build itself takes about 2 minutes to finish (beginning from installing Nix, to installing neuron, all the way to building your site). On top of that, there appears to be a lag in GitHub's actual deployment of the site. For instant deploy, keep an eye out for [Cerveau](https://neuron.zettel.page/041726b3.html).

What environment is used to build and deploy the site?
: From the [Actions workflow file](https://github.com/srid/neuron-template/blob/master/.github/workflows/publish.yaml), it can be seen that we install [neuron](https://neuron.zettel.page/) using Srid's Nix binary cache, as well as use [JamesIves/github-pages-deploy-action](https://github.com/JamesIves/github-pages-deploy-action) action to push the built site to the `gh-pages` branch, that in turn gets deployed to GitHub's servers.

Can I use my own domain name?
: Yes, see [GitHub's docs](https://help.github.com/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site).
