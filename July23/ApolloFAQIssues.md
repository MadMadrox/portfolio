# Issues and errors

## Table of contents
- [Conflicting file error](#conflicting-file-error)
- [Fork the repository and access denied](#fork-the-repository-and-access-denied)
- [Fix technical problems with a PR](#fix-technical-problems-with-a-pr)
- [Article sent back for correction](#article-sent-back-for-correction)
- [Made the requested corrections but article was sent back to me again](#made-the-requested-corrections-but-article-was-sent-back-to-me-again)
- [Creating self-help for topics not yet available](#creating-self-help-for-topics-not-yet-available)


## Conflicting file error

### Fixing a conflicting file error in Elixir
If there is a conflicting file error with one of the files in your PR, the best guidance is to discard and resubmit your changes through Elixir. File conflicts usually arise when the PR is old and the article you’re trying to edit has been changed by another PR/author. 

To discard your changes, save your changes locally (copy and paste to a text file/editor), select **Discard** in the action menu, and then submit a new PR.

### Fixing a conflicting file error in GitHub
1. Open your PR in GitHub.
2. Go to the **Files changed** tab.

![File changed tab](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_FilesChanged.PNG)

3. Select the ellipses (**...**) icon on the conflicting file, and select **Edit file**.

![Edit file option](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_EditFile.png)

4. Select all of your work and copy and paste it into an offline text file/editor (just to be safe).
5. Go back to the **Conversation** tab of your PR.

![Conversation tab](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_Conversations.PNG)

6. Scroll down to the bottom above the comments box, and you should see the conflicting file error message box.
7. Click the **Resolve conflicts** button on the right.

![Resolve conflicts button](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_00_ResolveConflicts.png)

8. A window will open showing the errors in the file. Don't worry about deleting each error. Parts of old commits may have been duplicated.

![Error 01](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_01_Error01.png)

![Error 02](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_02_Error02.png)

9. Select all of the content in the edit window and replace it by pasting the work you copied earlier.
10. Click the **Mark as resolved** button at the top right.

![Mark as resolved button](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_03_MarkAsResolved.png)

11. Click the green **Commit merge** button.

![Commit merge button](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_04_CommitMerge.png)

12. Back on the **Conversation** tab of your PR, scroll down and make sure the conflicting file error is gone, and the file is valid for merge.

![Conversation tab](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_Conversations.PNG)

![No more conflicts](https://github.com/MadMadrox/portfolio/blob/main/July23/ConflictingFileError/CFE_05_NoError.png)


Return to [Issues and errors: Table of contents](#table-of-contents).

## Fork the repository and access denied

If you are trying to fork the repository but keep getting access denied errors, you may not have completed all the steps outlined in the [**Self-help onboarding guide**](https://azsupportdocs.azurewebsites.net/portal/articles/SetupGithub.html).

Verify you have joined the:
-   [**Azure organization**](https://repos.opensource.microsoft.com/Azure)
-   [**Azure/SelfHelpContent repository**](https://github.com/Azure/SelfHelpContent)

Return to [Issues and errors: Table of contents](#table-of-contents).

## Fix technical problems with a PR

If you are experiencing problems with your PR, there are a few options to get help, depending on which stage the PR is in. 

|Status of PR|Where to find help|
|----|----------|
|**The PR has not been submitted for review.**<br>Any of the following conditions may apply to a PR that has not been submitted for review yet (but are not limited to these scenarios):<ul><li>The PR is stuck in Elixir</li><li>The PR is stuck in GitHub</li><li>The PR cannot be submitted for review (because of errors or other issues)</li></ul>|Post your question in the [Azure Customer Support Experiences channel](https://teams.microsoft.com/l/channel/19%3a9152bb360cd04d80adf257fbdc464cfa%40thread.skype/Azure%2520Customer%2520Support%2520Experiences?groupId=b63c0288-47e2-4861-898e-adcc9e288744&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47) and tag <strong>@ACPDevs</strong>. <strong>@ACPDevs</strong> are the engineers who work on Elixir and are the most familiar with issues preventing an article from being submitted for review.|
|**PR has been submitted for review**|<ol><li>Post your question in the [Azure Customer Support Experiences channel](https://teams.microsoft.com/l/channel/19%3a9152bb360cd04d80adf257fbdc464cfa%40thread.skype/Azure%2520Customer%2520Support%2520Experiences?groupId=b63c0288-47e2-4861-898e-adcc9e288744&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47), tag the <strong>@ACPTeam</strong> in your message, and include the PR link. The <strong>@ACPTeam</strong> is the team of editors who review all PRs and merge them for publication.</li><li>**Ping the editors on Teams.** Use the link you have to your PR on GitHub (Elixir should provide a link once a PR has been successfully submitted for review) and, on the **Conversation** tab, you should be able to see the history of sign-offs, comments, and labels associated with your PR. The name of the editor who reviewed your PR should be listed in the labels or in the history of the **Conversation** tab.<ul><li>Labels for authors will read like this: `Under-Review-By-EditorsName`</li><li>In the **Conversation** tab, an editor's GitHub alias (which is most likely also their name, but not in all cases) will be visible next to any activity they contributed to the PR. An editor contribution may be in the form of a comment or an added label.</li><li>A direct conversation with an editor may resolve your issue quicker than waiting for your PR to travel through the system again.</li></ul></li></ol>|

Return to [Issues and errors: Table of contents](#table-of-contents).

## Article sent back for correction

When an editor sends a PR back to the author for correction:

|Workspace|How to view the reason(s) for correction|
|---|------|
|In Elixir|You will have to manually check on the status of your PR to see if it was published or needs correction. If it needs correction, you will have to view the PR on GitHub to view the editor's comments.|
|In GitHub|<ul><li>A **Request-for-correction** tag is added to the PR.</li><li>On the **Files changed** tab of the PR, the comments made by the editor addressing the necessary corrections are displayed in the panes of the source view.<ul><li>Comments are usually placed as close to the source of the issue.</li><li>There may be more than one comment.</li><li>Be sure to scroll the length of the file to view all comments.</li></ul><li>On the **Conversation** tab, comments from the editor will also displayed but the entire history of changes to the PR is also displayed.</li><li>The **Conversation** tab is not as easy to scan for comments from an editor as the **Files changed** tab.</li></ul>

Articles may be sent back for correction for any of the following reasons:
- It does not meet the [minimum requirements for an Apollo article](https://azsupportdocs.azurewebsites.net/elixir/articles/MinRequirementsListApollo.html).
  - The article is missing a proper H2 title.
  - The article is missing an [informative description](https://azsupportdocs.azurewebsites.net/elixir/articles/TitleAndDescription.html) (aka. an introduction).
  - The article has a diagnostic and is missing [an informative description of what the diagnostic is performing and a description of the duration of the diagnostic check](https://azsupportdocs.azurewebsites.net/elixir/articles/Diagnostics.html).
- The editor needs the author to clarify some technical information either written by the author or revised by the editor.
- There is a [conflicting file error](#conflicting-file-error).
- The PR has validation errors only the author can resolve on their end.<!-- It would be nice to have a link to an official resource addressing validation errors. -->

Once you have reviewed the editor's comments and made corrections, you must resubmit the PR for the system to return the PR to the review team (editors).

|Workspace|Instructions to resubmit a PR|
|---|------|
|Working in Elixir|<ol><li>Re-open the PR in Elixir.</li><li>Select **Save**.</li><li>Select **Submit** to save your changes and resubmit your PR for review.</li></ol>|
|Working in GitHub|<ol><li>Open your PR in GitHub.</li><li>In the **Conversation** tab, scroll down to the comment box at the very bottom and type in `#sign-off`.</li><li>Select the green **Comment** button to resubmit your PR for review.</li></ol>|
<!-- Still need confirmation on these re-submitting processes -->

Return to [Issues and errors: Table of contents](#table-of-contents).

## Made the requested corrections but article was sent back to me again

Check for new editor comments. 
- The most likely reason for another request for correction is the information added was not specific enough. Titles, introductions, and descriptions should be tailored to the customer’s needs and address the content of the article. We want to provide customers with useful information that pertains to their scenario.
- The editor may have made changes to your revisions and require a confirmation of technical accuracy.
- New validation errors may have also occured.

Return to [Issues and errors: Table of contents](#table-of-contents).

## Creating self-help for topics not yet available

### Preview articles if the support topics are not in production

You can create content for any support topic if you have the SupportTopicId, even if the support topic is not enabled in production.

### New support topic trees

For multiple articles, submit a PR for the new self-help content before the new support topics are available in Prod. The validation process adds comments indicating the supportTopicId is invalid; however, that is not a blocker for the content review to start. Contact us in advance.

Return to [Issues and errors: Table of contents](#table-of-contents).
