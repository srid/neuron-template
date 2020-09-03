# How to publish your own [neuron](https://neuron.zettel.page/) site

[neuron](https://neuron.zettel.page/) is a Zettelkasten-based notes manager, and you can use this template repository to get started with [publishing](https://neuron.zettel.page/778816d3.html) your own neuron site that looks like [one of these](https://neuron.zettel.page/2013101.html).

- Go to <https://github.com/srid/neuron-template/generate>
- Give your new repository a name, say `mynotes`
- Select "*Include all branches*" ([necessary to get the site to publish](https://stackoverflow.com/a/47368231/55246))
- Click "Create repository from template"
  - Note: if you are on the free GitHub plan, your repository should be public for GitHub to publish it.

GitHub will now build the site, which will become available at `https://<yourgithubusername>.github.io/mynotes/`.

For more information, see [neuron documentation](https://neuron.zettel.page/) as well as the [GitHub Pages guide](https://help.github.com/en/github/working-with-github-pages).

## Set your site metadata

- In your new repository, edit the `neuron.dhall` file to set your site configuration (such as title, author, color theme) to suitable values.

## How to edit and add notes

Assuming you have changed the `editUrl` configuration in `neuron.dhall` (see the above section), you can simply click the "edit" icon on the published site to edit any note (see [Editing files in your repository](https://help.github.com/en/github/managing-files-in-a-repository/editing-files-in-your-repository) and [Creating new files](https://help.github.com/en/github/managing-files-in-a-repository/creating-new-files)). On every change, your site should eventually rebuild.

To understand how linking works, read [the neuron guide on Linking](https://neuron.zettel.page/2011504.html).

For other ways to edit your notes (editors, web interface), see the [neuron guide](https://neuron.zettel.page/2011406.html). In particular, [Cerveau](https://www.cerveau.app/) is the easiest way to edit your notes on the go.

Questions? Checkout the [[faq]].