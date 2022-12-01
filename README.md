<!-- Title -->
<p align="center">
	<img src="docs/images/logo-transparent.svg" alt="Logo" width="250" height="80">
</p>

# Support Docs


<!-- TABLE OF CONTENTS -->
<div>
	<summary><h2 style="display: inline-block">Table of Contents</h2></summary>
	<ol>
		<li><a href="#about-the-project">About The Project</a></li>
		<li>
			<a href="#getting-started">Getting Started</a>
			<ul>
				<li><a href="#generating-a-github-ssh-key">Generating a GitHub SSH key</a></li>
				<li><a href="#installation">Installation</a></li>
			</ul>
		</li>
		<li><a href="#usage">Usage</a></li>
	</ol>
</div>


<!-- ABOUT THE PROJECT -->
## About the Project

This is repo holds all of Specific Energy's public facing documentation.
<br />
**Built with:** Mkdocs


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Generating a GitHub SSH key
_[More info from GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)_
<br />

1. Create a passphrase using the random password generator of your choice.

2. Generate an ssh key
	<br />
	```ssh-keygen -t ed25519 -C "your_email@example.com"```

3. Start the ssh-agent in the background.
	<br />
	```eval "$(ssh-agent -s)"```

4. Add your SSH key to the ssh-agent
	<br />
	```ssh-add ~/.ssh/id_ed25519```

5. [Add the SSH key to your account on GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)


### Installation

1. Clone the repo
	<br />
   ```git clone git@github.com:Specific-Energy/support-docs.git```

2. Run the init script
   ```./init.sh```


<!-- USAGE -->
## Usage

To add a new page:  <br />

1. Add the page as a ```.md``` file in docs
	- If the file is nested: ```folder/new-file.md``` 
2. Add the page in the ```mkdocs.yml``` under ```nav:```

<br />

**To run the project locally:**  <br />
```mkdocs serve```

**To deploy:**  <br />
```mkdocs gh-deploy```