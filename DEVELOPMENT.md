# Development Guide for KU-BioML website

## Download and setup
1. **Clone the repository**:
    First, you need to clone the repository to your local machine. 

    ```bash
    git clone https://github.com/KU-BioML/KU-BioML.github.io.git
    ```
2. **Initialize Submodules**:
    The repository uses a submodule for the theme. You need to initialize the submodule before you can build the website. 

    ```bash
    cd KU-BioML.github.io # Go to the root directory of the repository
    git submodule update --init --recursive
    ```
3. **Install Hugo**:
    If you haven't installed Hugo already, follow the [official installation guide](https://gohugo.io/installation/).

## Development
1. **Create a New Branch**:
   Before making any changes, create a new branch:
   
   ```bash
   git checkout -b [your-branch-name]
   ```

2. **Start Local Server**:
   Navigate to your repository's root directory and start the Hugo server:
   
   ```bash
   hugo server -D
   ```

   The `-D` flag ensures that draft content is also displayed. You should now be able to access your site at `http://localhost:1313/`.

3. **Content Creation**:
   To create a new content page, use:
    ```bash
    hugo new content/[section-name]/[new-content-name].md
    ```

    Replace `[section-name]` with the section where you want the content to be (e.g., `News`, `People`) and `[new-content-name]` with the desired name for your new content.

4. **Layouts and Design**:
   - You can modify existing layouts or create new ones inside the `layouts` directory.
   - For basic styling or adding scripts, you can modify the theme directly or add files to the `static` directory.

5. **Images and Assets**:
   - Place images inside the `static/images` directory.
   - For article-specific images, use the `static/images/articles` directory.
   - Social media icons and assets can be placed in the `static/social` directory.

6. **Committing Changes and Creating a Pull Request**:
   After making changes, commit them to your branch and then push the branch to your repository:

   ```bash
   git add .
   git commit -m "Description of changes made"
   git push origin [your-branch-name]
   ```

   Once your branch is pushed, go to your GitHub repository and create a pull request against the `master` branch. The workflows will ensure that the website is tested and then automatically deployed upon merging the pull request.

## GitHub Workflows

There are two main GitHub workflows associated with this repository:

1. **Build Hugo Site Workflow**: This workflow tests that building the website works. It is triggered on every push to the repository.
   File: `build_hugo.yml`

2. **Deploy Hugo Site to Pages Workflow**: This workflow builds and deploys the Hugo site to GitHub Pages. It is triggered on pushes to the `master` branch or can be run manually from the Actions tab.
   File: `deploy_hugo.yml`