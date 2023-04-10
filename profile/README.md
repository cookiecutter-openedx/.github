# Welcome to Cookiecutter Open edX

[![discuss.overhang.io](https://img.shields.io/static/v1?logo=discourse&label=Forums&style=flat-square&color=ff0080&message=discuss.overhang.io)](https://discuss.overhang.io)
[![docs.tutor.overhang.io](https://img.shields.io/static/v1?logo=readthedocs&label=Documentation&style=flat-square&color=blue&message=docs.tutor.overhang.io)](https://docs.tutor.overhang.io)<br/>
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)

## How it works

Powered by [Cookiecutter](https://github.com/cookiecutter/cookiecutter), Cookiecutter Open edX is a community maintained project for jumpstarting and managing production-ready [Tutor](https://docs.tutor.overhang.io/) and [Kubernetes](https://kubernetes.io/) based installations of the [Open edX:tm: online learning management system](https://openedx.org/) running on [AWS](https://aws.amazon.com/) cloud infrastructure that is built and managed with fully parameterized [Terraform](https://www.terraform.io/) and [Github Actions](https://docs.github.com/en/actions) automation scripts.

![Cookiecutter workflow](https://github.com/cookiecutter-openedx/.github/blob/main/doc/cookiecutter-how-it-works.png)

The cookiecutter project helps you to remain focused on the blue boxes by providing you with templated solutions for everything else.

To provide a consistent onboarding experience to new Cookiecutter users we also manage a few other repositories on which the automated build and deployment workflows depend. These include:

- an [Open edX Plugin](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin) that contains modifications that are needed when installing Open edX:tm: to Kubernetes.
- a collection of [tutor plugins](https://docs.tutor.overhang.io/tutorials/plugin.html) that are needed when installing Open edX:tm: to Kubernetes.
- a [Github Action](https://github.com/cookiecutter-openedx/aws-ecr-create) that automatically creates [AWS Elastic Container Repositories](https://aws.amazon.com/ecr/) for you if they're referenced in your workflow.
- any repositories which we've forked on an interim basis in order to facilitate Kubernetes-specific customizations, the PR's of which are pending in their respective upstream repositories.

Additionally, we maintain the following repositories that include working code samples and best practices for customizing and extending the feature set of Open edX installations:

- an example [Open edX plugin](https://github.com/cookiecutter-openedx/openedx-plugin-example) that includes working, maintained code samples illustrating how to accomplish various programming and integration tasks.
- an example [Open edX custom theme](https://github.com/cookiecutter-openedx/openedx-theme-example) that provides scaffolding to help you get started with cusomizing the appearance of your Open edX:tm: platform

And finally, if you use Wordpress as your marketing site then we also maintain the following projects:

- a custom Open edX Third Party [oAuth backend for Wordpress](https://github.com/cookiecutter-openedx/edx-oauth2-wordpress-backend).
- an [Open edX Plugin](https://github.com/cookiecutter-openedx/django-memberpress-client) that implements a Wordpress memberpress REST API client.

## Our commitment to the Open edX community

We want to make it easier and more economical for small educational institutions, non-profits and ed-tech companies to leverage Open edX:tm: software. A single technology enthusiast should be able to maintain an Open edX:tm: platform on a part-time basis. Typical platforms should incur less than $500 usd in monthly cloud infrastructure costs.

## Our mission and philosophy

Online learners are accustomed to performant, reliable and safe user experiences across the Internet, and they expect the same from your platform. But infrastructure and systems management are complex, constantly evolving matters that are hard to do well, and they don't provide any meaningful differentation for your project. Compounding matters, installing and configuring Open edX:tm: software is notoriously complex; even more so if you need to run your platform at scale. Lastly, keeping packaged software and infrastructure properly maintained is hard work. Cloud infrastructure providers evolve and the back end services they offer undergo routine updates. Open edX:tm: releases new features. New security threats surface on a regular basis.

**We believe that these are problems best solved by the Open edX community and that Cookiecutter Open edX's templated infrastructure-as-code strategy is the best way to facilitate this.**

## History

The Cookiecutter Open edX project was originally conceived in 2021 by project members working on the [Government Communications eLearning](https://staging.global-communications-academy.com/) project for the [UK Cabinet Office](https://www.gov.uk/government/organisations/cabinet-office) which they generously open-sourced. The principal project maintainer is [Lawrence McDaniel](https://lawrencemcdaniel.com/), a full stack developer and [Open edX community blogger](https://blog.lawrencemcdaniel.com/).

The Government Communications eLearning platform was one of the first Docker-based Open edX:tm: platforms to launch at scale on Kubernetes-based cloud infrastructure. The devops team from this project brought a wealth of knowledge about cloud infrastructure, Kubernetes, CI/CD and infrastructure-as-code. Their efforts led to a robust set of integrated Terraform modules and fully automated CI solutions for building and deploying Open edX:tm: to Kubernetes. Moreover, they codified their extensive knowledge of CI and Kuberenetes best practices, maximizing the potential of these evolving technologies. In early 2022 this codebase was refactored into a more generalized collection of Jinja templating tools now known as "Cookiecutter Open edX" that is more suitable for community use and provides easy onboarding. Since then, the scope and feature set of Cookiecutter Open edX has grown considerably.

## Get involved

Contributors are welcome! Contact me here: [lawrencemcdaniel.com](https://lawrencemcdaniel.com/contact) if you're interested in becoming a contributor to this project.

## Open edX Github Actions

Don't forget to take a look at our cousin organization [Open edX Github Actions](https://github.com/openedx-actions) where we manage a collection of several dozen [Github Actions](https://github.com/features/actions) components that are used to create our automated Build and Deploy workflows.
