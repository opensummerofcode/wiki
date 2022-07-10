---
description: How to deploy and host your project ?
---

# Deployment

## Hosting

### Static website

Most projects can be built as a static website.

In this case, we recommend using platforms that can deploy your website for free.

Here are a few suggestions, but feel free to deploy your website using another solution:

{% tabs %}
{% tab title="Netlify" %}
[https://docs.netlify.com/welcome/add-new-site/](https://docs.netlify.com/welcome/add-new-site/)
{% endtab %}

{% tab title="Heroku" %}
[https://devcenter.heroku.com/articles/github-integration](https://devcenter.heroku.com/articles/github-integration)
{% endtab %}

{% tab title="Vercel" %}
[https://vercel.com/docs/concepts/deployments/overview](https://vercel.com/docs/concepts/deployments/overview)
{% endtab %}

{% tab title="GitHub Pages" %}
Even though, it's possible to use GitHub Pages to deploy your project, we recommend not to use it because it will be used to deploy the page to present your project (during Week 4).

Example: [https://osoc21.github.io/BikeInfrastructure/](https://osoc21.github.io/BikeInfrastructure/)
{% endtab %}
{% endtabs %}

Contact you coach or osoc technical support if you need help to deploy your static website.

### Docker container(s)

Some projects need something a bit more complicated.\
For instance, you need to deploy your own API and the front-end.

Your Docker container(s) will be deployed using [Digital Ocean App Platform](https://www.digitalocean.com/products/app-platform).

Documentation:

* [https://docs.digitalocean.com/products/app-platform/](https://docs.digitalocean.com/products/app-platform/)
* [https://docs.digitalocean.com/products/app-platform/reference/dockerfile/](https://docs.digitalocean.com/products/app-platform/reference/dockerfile/)

⚠️ Digital Ocean App Platform does **not** support Docker Composer.

Contact you coach or osoc technical support if you need help to create the Docker container or deploy your Docker container.

### Server / Droplet

If creating a Docker container is not option, we can give you `root` access to a Debian/Ubuntu server dedicated to your project and hosted in OKBE infrastructure.

This solution is not recommended and will have to be discussed with osoc technical support and OKBE infrastructure manager.

This server will be a [Digital Ocean Droplet](https://www.digitalocean.com/products/droplets) with the following setup:

* Memory: 1GB
* CPU: 1vCPU
* Transfer: 1TB
* SSD: 25GB

## Domain name

### Sub-domain \*.osoc.be

We offer an `osoc.be` sub-domain name for your project.\
We usually create a sub-domain name with the name of your project : \
`your-team-name.osoc.be`

If your project needs multiple sub-domains, it's of course possible!

Example:

* `your-team-name.osoc.be` for the front-end
* `api.your-team-name.osoc.be` for the API
* ...

Once your project is deployed, contact osoc technical support with the IP address or CNAME record, so we can create the sub-domain name and link it to your project.

{% tabs %}
{% tab title="Netlify" %}
[https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/](https://docs.netlify.com/domains-https/custom-domains/configure-external-dns/)
{% endtab %}

{% tab title="Heroku" %}
[https://devcenter.heroku.com/articles/custom-domains](https://devcenter.heroku.com/articles/custom-domains)
{% endtab %}

{% tab title="Vercel" %}
[https://vercel.com/docs/concepts/projects/custom-domains](https://vercel.com/docs/concepts/projects/custom-domains)
{% endtab %}

{% tab title="GitHub Pages" %}
[https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages)
{% endtab %}
{% endtabs %}

### Domain name

We do not offer domain names but if your client offers a domain name (example from a previous year: [https://routeplanner.bike.brussels/](https://routeplanner.bike.brussels/)), give your client the IP address or CNAME record so they can configure the domain name correctly.
