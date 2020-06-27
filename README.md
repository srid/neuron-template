# How to create your own neuron site

- Go to <https://github.com/srid/neuron-template> and click the "*Use this template*" button
  - Give your repository a name, say `mynotes`
  - Select "*Include all branches*" ([necessary to get the site to publish](https://stackoverflow.com/a/47368231/55246))

GitHub will now build the site, which will become available at `https://<yourgithubusername>.github.io/mynotes/`.

For more information, see the [GitHub Pages guide](https://help.github.com/en/github/working-with-github-pages).

## Set your site metadata

- In your new repository, edit the `neuron.dhall` file to reflect your new site.

## How to edit and add notes

Assuming you have changed the `editUrl` in `neuron.dhall` (see above), you can simply click the "edit" icon on the publish site to edit any note. To create a *new* note, use the GitHub interface. On every change, your site should eventually rebuild.

For other ways to edit your notes, see the [neuron guide](https://neuron.zettel.page/2011406.html).
