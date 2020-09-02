你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
Terraform Provider for Google Cloud Platform
==================

- Website: https://www.terraform.io
- Documentation: https://www.terraform.io/docs/providers/google/index.html
- [![Gitter chat](https://badges.gitter.im/hashicorp-terraform/Lobby.png)](https://gitter.im/hashicorp-terraform/Lobby)
- Mailing list: [Google Groups](http://groups.google.com/group/terraform-tool)
<img src="https://cdn.rawgit.com/hashicorp/terraform-website/master/content/source/assets/images/logo-hashicorp.svg" width="600px">

Maintainers
-----------

This provider plugin is maintained by:

* The [Google Cloud Graphite Team](https://cloudplatform.googleblog.com/2017/03/partnering-on-open-source-Google-and-HashiCorp-engineers-on-managing-GCP-infrastructure.html) at Google
* The Terraform team at [HashiCorp](https://www.hashicorp.com/)

Requirements
------------

-	[Terraform](https://www.terraform.io/downloads.html) 0.10+
-	[Go](https://golang.org/doc/install) 1.11.0 or higher


Using the provider
----------------------

See the [Google Provider documentation](https://www.terraform.io/docs/providers/google/index.html) to get started using the
Google provider.

We recently introduced the `google-beta` provider. See [Provider Versions](https://www.terraform.io/docs/providers/google/provider_versions.html)
for more details on how to use `google-beta`.

Upgrading the provider
----------------------

The Google provider doesn't upgrade automatically once you've started using it. After a new release you can run 

```bash
terraform init -upgrade
```

to upgrade to the latest stable version of the Google provider. See the [Terraform website](https://www.terraform.io/docs/configuration/providers.html#provider-versions)
for more information on provider upgrades, and how to set version constraints on your provider.

Building the provider
---------------------

Clone repository to: `$GOPATH/src/github.com/terraform-providers/terraform-provider-google`

```sh
$ mkdir -p $GOPATH/src/github.com/terraform-providers; cd $GOPATH/src/github.com/terraform-providers
$ git clone git@github.com:terraform-providers/terraform-provider-google
```

Enter the provider directory and build the provider

```sh
$ cd $GOPATH/src/github.com/terraform-providers/terraform-provider-google
$ make build
```

Developing the provider
---------------------------

If you wish to work on the provider, you'll first need [Go](http://www.golang.org) installed on your machine (version 1.11.4+ is *required*). You'll also need to correctly setup a [GOPATH](http://golang.org/doc/code.html#GOPATH), as well as adding `$GOPATH/bin` to your `$PATH`.

To compile the provider, run `make build`. This will build the provider and put the provider binary in the `$GOPATH/bin` directory.

```sh
$ make build
...
$ $GOPATH/bin/terraform-provider-google
...
```

For guidance on common development practices such as testing changes or vendoring libraries, see the [contribution guidelines](https://github.com/terraform-providers/terraform-provider-google/blob/master/.github/CONTRIBUTING.md). If you have other development questions we don't cover, please file an issue!
