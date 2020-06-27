# Example Zettelkasten

This is a template zettelkasten for [neuron](https://neuron.zettel.page/). It supports deploying to GitHub Pages on every git push to `master` branch in GitHub.

## How to fork

- Go to <https://github.com/srid/neuron-template> and click "Use this template" button
- In your new repository, edit the `neuron.dhall` and change someting (i.e., the title)
- WIP: ??? 

GitHub will now build the site, which will become available at `https://<yourgithubusername>.github.io/<yournewrepo>/`.

## FAQ

Why does the site not update instantly?
:  The [GitHub Actions](https://github.com/features/actions) build itself takes about 2 minutes to finish (beginning from installing Nix, to installing neuron, all the way to building your site). On top of that, there appears to be a lag in GitHub's actual deployment of the site. For instant deploy, keep an eye out for [Cerveau](https://neuron.zettel.page/041726b3.html).
