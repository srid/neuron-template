# neuron-template

## How to use

- Go to <https://github.com/srid/neuron-template> and click "Use this template" button
  - Select "Include all branches" (necessary to get the site to publish)
- Optional: In your new repository, edit the `neuron.dhall` file and change something (eg. the title)

GitHub will now build the site, which will become available at `https://<yourgithubusername>.github.io/<yournewrepo>/`.

## How to edit

Assuming you have changed the `editUrl` in `neuron.dhall`, you can simply click the "edit" icon on the publish site to edit any note. To create a *new* note, use the GitHub interface. On every change, your site should eventually rebuild.

## FAQ

Why does the site not update instantly?
:  The [GitHub Actions](https://github.com/features/actions) build itself takes about 2 minutes to finish (beginning from installing Nix, to installing neuron, all the way to building your site). On top of that, there appears to be a lag in GitHub's actual deployment of the site. For instant deploy, keep an eye out for [Cerveau](https://neuron.zettel.page/041726b3.html).
