+++
title = "Chart Repository FAQ"
weight = "8"

tags = ["charts", "repo", "faqs"]
section = "developing-charts"
categories = ["developing-charts"]
type = "page"

slug = "chart-repo-faq"

[menu.main]
  url = "chart-repo-faq"
  parent = "developing-charts"

+++

# Chart Repositories: Frequently Asked Questions

This section tracks some of the more frequently encountered issues with using chart repositories.

**We'd love your help** making this document better. To add, correct, or remove
information, [file an issue](https://github.com/kubernetes/helm/issues) or
send us a pull request.

## Fetching

**Q: Why do I get a `unsupported protocol scheme ""` error when trying to fetch a chart from my custom repo?**

A: This is likely caused by you creating your chart repo index without specifying the `--url` flag.
Try recreating your `index.yaml` file with a command like `heml repo index --url http://my-repo/charts .`,
and then re-uploading it to your custom charts repo.