# forecasting-model

## How to Create a Branch

To create a new branch in this repository, you can use one of the following methods:

### Using Git Command Line

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone https://github.com/Atabak-Touri/forecasting-model.git
   cd forecasting-model
   ```

2. **Create and switch to a new branch**:
   ```bash
   git checkout -b your-branch-name
   ```
   Or using the newer Git syntax:
   ```bash
   git switch -c your-branch-name
   ```

3. **Push the branch to GitHub**:
   ```bash
   git push -u origin your-branch-name
   ```

### Using GitHub Web Interface

1. Navigate to the repository at https://github.com/Atabak-Touri/forecasting-model
2. Click on the branch dropdown button (displays the current branch name, e.g., "main")
3. Type your desired branch name in the search/create text field
4. Click the "Create branch: [your-typed-name]" option that appears below

### Using GitHub CLI

If you have the [GitHub CLI](https://cli.github.com/) installed:
```bash
# Clone the repository (if you haven't already)
gh repo clone Atabak-Touri/forecasting-model
cd forecasting-model

# Create and switch to a new branch
git checkout -b your-branch-name
# Or using the newer syntax:
git switch -c your-branch-name

# Push the branch to GitHub
git push -u origin your-branch-name
```