# greenwood-library-website

> # Enhancing a Community library website

> ## Background Scenario

As part of a development team tasked with enhancing the website for the **"Greenwood Community Library."** The website aims to be more engaging and informative for its visitors. It currently includes basic sections: **Home**, **About is**, **Events**, **and Contact Us.** The team has decided to add a **"Book Reviews"** section and update the **"Events"** page to feature upcoming community events.

I will simulate the roles of two contributors: **"Morgan"** and **"Jamie"**. Morgan will focus on adding the **"Book Reviews"** section, while Jamie will update the **"Events"** page with new community events.

> ## Setup 

1. Create a Repository on GitHub:

- Sign up or log into [GitHub](https://github.com/login).
- Click the "+" icon in the top-right corner and select "New repository".

![New_repo](img/1.create_repo.png)

- Name the repository **greenwood_library-website**, make it public (optional ) and initialize it with a README file.
- Click "Create repository"

![Create_repo](img/2.name_repo.png)

- On the repository's page on GitHub, click the "Code" button and copy the HTTPS URL.

![Clone_repo](img/3.clone_repo.png)

- Open your terminal or command prompt.
- Clone (Download) the repository from GitHub using;

  `git clone [paste the URL copied from GitHub]`
  ![Clone_repo](img/3.1.clone_repo..png)

> ## Tasks

1. In the main branch, using Visual Studio Code editor ensure there are files for each of the web pages; **home.html, about_us.html, events.html, contact_us.html**.

- Navigate into the clonned repository:

`cd greenwood-library-website/`

![Clone_repo](img/4.0.change_dir.png)

- Open Visual Studio Code editor and expand **greenwood-library- website** to view files in it:
  ![View _files](img/4.1.view_files_vscode.png)

2. Add any random content into each of the files.

- Add random content into each of the files:
  ![Add_content](img/5.0.AddContentToFile.png)

- check content added:
  ![Add_content](img/5.%20AddContentToFile.png)

- check changes has not been staged:

  `git status`

![Add_content](img/6.check_status.png)

The files appear in **red** showing that changes have been made to the file and ready for staging.

3. Stage, commit and push the changes directly to the **main** branch.

- stage changes and confirm changes have been staged for commit:

`git add about_us.html contact-us.html events.html home.html`

`git status`

![Stage](img/7.stage.png)

After stages have been made, the file names will appear **green** in the terminal output. This colour change signifies that the file has been succesfully staged and ready for committing.

- Commit changes that have been staged for commit:

`git commit -m "about_us commit"`
![Commit](img/8.commit.png)

- Push main branch to Github:

`git push origin main`
![Push](img/9.push.png)

> ## Morgan's Work: Adding Book Reviews

1. Create a Branch for morgan.

- Navigate to the cloned project directory:
  `cd greenwood-library-website`

- Check the current branch:

`git branch`
![check-branch](img/10.%20check%20branch.png)
Initially, you'll see **"main"** as the only branch being the default starting point without other branches crated yet.

- Create a new branch for Morgan's work:

`git checkout -b add-book-reviews`

- Check the branch to see newly created branch:

`git branch`

![create-branch](img/11.create_branch_add-book-reviews.png)

2. Switch to a new branch named **add-book-reviews**.

Running **git branch** again now shows your newly created branch, indicating you're now working in the new **"workspace"** dedicated to Morgan's updates.

3. Add a new file **book_reviews.html** to represent the Book Reviews Section.

`touch book_reviews.html`
![add-book-reviews](img/12.add_book-reviews.png)

4. Add a random text content into the file.

- In VS Code, select **book_reviews.html** file and add text in the opened tab.
  ![Add-content](img/12.1.add_Content_book-review.png)

- Check that changes have not been staged

`git status`
![chech-status](img/13.1.check-status.png)

At this stage, Morgan has modified the file, but the changes haven't been prepared for a commit in Git, indicated by the file name appearinf in **red** in the terminal output, signaling that changes are recognized by Git but not yet staged.

5. Stage, commit, and Push Changes with a message like **"Add book reviews section."**

- Stage Morgan's changes:

`git add book_reviews.html`
![stage-changes](img/13.2.Stage_book-review.png)

- Confirm Morgan's changes have been staged:

`git status`
![Confirm-staging](img/13.3.Confirm-staging.png)

- Commit morgan's changes:

`git commit -m "add book review"`
![Commit-changes](img/14.commit_book-review.png)

6. push the **add-book-reviews** branch to Github.

- Push Morgan's branch to Github:

`git push origin add-book-reviews`
![Push-to-Github](img/15.push_book-review.png)

7. Raise a PR for Morgan's Work.

- Open web browser and go to the GitHub page for the repository.
- click on the branch dropdown menu near the top left corner of the file list and select **add book review** branch.
  ![Morgan-branch](img/16.PR_morgan.png)
- Click the "New pull request" button next to the branch dropdown menu:
  ![Open-PR](img/16.1.png)

8. Merge Morgan's work to the **main** branch.

- Create pull request:
  ![Create-PR](img/16.2.png)
- Review and merge pull request:
  ![Merge-PR](img/16.3.png)
- Confirm pull request:
  ![Confirm-PR](img/16.4.png)
- Pull request successfully merged and closed:
  ![Merge-confirmed](img/16.5.png)

> ## Jamie's Work: Updating Events page

Repeat the same flow for Jamie's work on Events Page. Ensure Jamie's work is in **update-events** branch.

- Pull the latest changes from the main branch into **update-events** before raising the PR.

![Checkout_main-jamie](img/17.git_checkout_main-jamie.png)
![Git_Pull-main](img/18.git_pull_main.png)
![Create-branch](img/19.create_branch_jamie.png)
![Update-content](img/20.update_content.png)
![Push_Update-events](img/21.push_update-events.png)
![create-PR](img/22.PR.png)
![Open-PR](img/22.1.open_PR.png)
![Create_PR](img/22.2.create_PR.png)
![Merge_PR](img/22.3.merge_PR.png)
![Confirm-merge](img/22.4.confirm-merge_PR.png)
![Merge-successful](img/22.5.PR_successful.png)
