                        TERRAFORM

What is Terraform?

Terraform is a popular cloud orchestration tool in the world of automation, which is used to deploy your infrastructure through the IAC (Infrastructure as code) approach.

Terraform is built by Hashicorp and released under Mozilla Public License. It supports public, private as well and hybrid cloud, as of now Terraform supports 145 providers, which include popular providers like AWS, Azure Cloud, GCP, Oracle Cloud, and many others.

Terraform architecture is very simple. All you need is to download the terraform binary to your local/server machine which is going to act as your base machine.

We have to mention the provider to work within our syntax file. Terraform will download the plugin for that particular provider automatically and will authenticate with the provider API to execute the plan.

What is Infrastructure as Code?

The process of provisioning and managing resources like Virtual Machines, Storage, Networks, Database, etc.. through machine-readable definition files, rather than interactive tools or hardware configurations.

Features

Open-source.
Declarative syntax.
Pluggable Modules.
Immutable infrastructure.
Simple client-only architecture.

Let’s get started…

Installing Terraform in Linux Distributions
The Terraform primary distribution packages come in .zip format, that includes single executable files that you can uncompress at any location on your Linux system.

However, for simpler integration with configuration management tools, terraform also offers package repositories for Debian-based and RHEL-based systems, which enables you to install Terraform using your default package management tools called APT, Yum, or DNF.

Install Terraform in Debian, Ubuntu & Mint


wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update 
sudo apt install terraform


Install Terraform in RHEL and CentOS

sudo dnf install -y dnf-plugins-core
sudo dnf config-manager --add-repo https://rpm.releases.hashicorp.com/fedora/hashicorp.repo
sudo dnf update
sudo dnf -y install terraform

Now the installation can be verified by running a simple terraform version command

$ terraform version

That’s it for this article. The installation is very simple and easy to set up and some text editors like Sublime and VSCode come with language support for Terraform too.

