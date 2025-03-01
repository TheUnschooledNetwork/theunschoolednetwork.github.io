# The Unschooled Network

[![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy)][gem]&nbsp;
[![GitHub license](https://img.shields.io/github/license/cotes2020/chirpy-starter.svg?color=blue)][mit]

Welcome to The Unschooled Network! This repository contains the source code for our website, built using Jekyll and the Chirpy theme.

## Usage

Check out the [theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki) for detailed information on how to use the Chirpy theme.

## Contributing

We welcome contributions from the community! To get started, please follow our [Contributing Guide](https://theunschoolednetwork.github.io/posts/2025-02-14-Contributing-to-Unschooled/). This guide will walk you through the process of setting up your environment, creating a new post, and submitting a Pull Request.

### Quick Start

1. **Set up the necessary tools**:
    ```bash
    sudo apt update
    sudo apt install ruby-full build-essential zlib1g-dev git
    ```

2. **Configure Ruby Gems** (if using Bash):
    ```bash
    echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
    echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
    echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
    source ~/.bashrc
    ```

3. **Install Jekyll and Bundler**:
    ```bash
    gem install jekyll bundler
    ```

4. **Clone the repository and install dependencies**:
    ```bash
    git clone https://github.com/TheUnschooledNetwork/theunschoolednetwork.github.io.git
    cd theunschoolednetwork.github.io
    bundle install
    ```

5. **Create a new branch**:
    ```bash
    git checkout -b my-new-post
    ```

6. **Add a new post**:
    Navigate to the [_posts](http://_vscodecontentref_/2) directory and create a new Markdown file following the naming convention:
    ```bash
    cd _posts
    nano YYYY-MM-DD-title-of-your-post.md
    ```

    Use the following front matter template at the top of your file:
    ```yml
    ---
    title: "Your Post Title"
    date: YYYY-MM-DD HH:MM:SS -500
    categories: [your-category]
    tags: [your-tags]
    ---
    ```

7. **Preview your changes locally**:
    ```bash
    bundle exec jekyll serve
    ```
    Open `http://localhost:4000` in your browser to check your changes.

8. **Commit and push your changes**:
    ```bash
    git add _posts/YYYY-MM-DD-title-of-your-post.md
    git commit -m "Draft: Initial version of 'My Post Title'"
    git push origin my-new-post
    ```

9. **Submit a Pull Request**:
    Open a browser and navigate to [TheUnschooledNetwork.github.io](https://github.com/TheUnschooledNetwork/theunschoolednetwork.github.io) repository. Click the "Compare & pull request" button, fill out the PR details, and submit.

For more detailed instructions, please refer to our [Contributing Guide](https://theunschoolednetwork.github.io/posts/2025-02-14-Contributing-to-Unschooled/).

## License

This work is published under [MIT][mit] License.

[gem]: https://rubygems.org/gems/jekyll-theme-chirpy
[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy/
[mit]: https://github.com/cotes2020/chirpy-starter/blob/master/LICENSE