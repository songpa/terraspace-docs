<div align="center">
  <a href="https://terraspace.cloud"><img src="https://img.boltops.com/boltops/logos/terraspace-dark-v2.png" /></a>
</div>

# Terraspace Documentation

This project powers the terraspace documementation website: [https://terraspace.cloud](https://terraspace.cloud).  It is a static website generated by [Jekyll](https://jekyllrb.com/).

## Contributing

For minor changes like typos, you can click **Suggest an edit to this page**, located at the bottom of each article. This will take you to the source file on GitHub, where you can submit a pull request for your change through the UI.

## Local Setup

For larger fixes, you can run the site locally with the following:

    git clone https://github.com/boltops-tools/terraspace-docs.git
    cd terraspace-docs
    bundle
    foreman start

You'll be able to view the site on [http://localhost:4000](http://localhost:4000).

## Html Proofer

Run it locally once in a while. Sometimes external sites are intermittently down, even GitHub.

    bundle exec rake html:proof