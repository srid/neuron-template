# How to publish your own [neuron](https://neuron.zettel.page/) site


- Go to <https://github.com/srid/neuron-template/generate>
- Give your repository a name, say `mynotes`
- Select "*Include all branches*" ([necessary to get the site to publish](https://stackoverflow.com/a/47368231/55246))
- Click "Create repository from template"

GitHub will now build the site, which will become available at `https://<yourgithubusername>.github.io/mynotes/`.

For more information, see the [GitHub Pages guide](https://help.github.com/en/github/working-with-github-pages).

## Set your site metadata

- In your new repository, edit the `neuron.dhall` file and update the neuron configuration to suitable values.

## How to edit and add notes

Assuming you have changed the `editUrl` configuration in `neuron.dhall` (see the above section), you can simply click the "edit" icon on the published site to edit any note (see [Editing files in your repository](https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository) and [Creating new files](https://help.github.com/en/github/managing-files-in-a-repository/creating-new-files)). On every change, your site should eventually rebuild.

For other ways to edit your notes, see the [neuron guide](https://neuron.zettel.page/2011406.html).
