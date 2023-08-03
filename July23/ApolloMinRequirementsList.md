# Minimum requirements checklist for Solutions 2.0 (Apollo) articles

To make sure that your article is ready for review, check each of the following items and verify that your article meets the requirement. 
- If your article doesn’t meet these minimum requirements, our editors will return the article to you. 
- By meeting these requirements, you’ll expedite the review-to-publish process for your article. 

**Articles that don't meet these requirements will be sent back for correction.**

For additional guidance on any of these items, see the [authoring guidelines](ApolloFAQOverview.md). Also, be sure to review the [Apollo template](https://github.com/Azure/SelfHelpContent/blob/master/documents/SelfHelp-Solution-template/apollo-markdown-template.md) if you've never written an Apollo article before, or need a reference.
  

## New articles

**Any new article must follow the requirements below. Also, consider the following recommended tips for improving your article.**

### Required
:heavy_check_mark: **Properties metadata section** is complete.

:heavy_check_mark: **Article title (header 2 tag)** that [starts with an active, imperative verb or verb phrase](https://azsupportdocs.azurewebsites.net/elixir/articles/TitleAndDescription.html) (“Resolve,” “Troubleshoot,” “Learn to”). 

:heavy_check_mark: **Introduction** that [describes the issue, offers examples of use cases and root causes where applicable, and provides basic context](https://azsupportdocs.azurewebsites.net/elixir/articles/TitleAndDescription.html).  


:heavy_check_mark: **Article body** includes, at minimum, an introduction and one or more solution components: manual troubleshooting steps, FAQ, [Azure Monitor charts](https://azsupportdocs.azurewebsites.net/elixir/articles/AzureMonitor.html), [custom data charts](https://azsupportdocs.azurewebsites.net/elixir/articles/CustomDataCharts.html), [metrics](https://azsupportdocs.azurewebsites.net/elixir/articles/AzureMonitor.html), [videos](https://azsupportdocs.azurewebsites.net/elixir/articles/Video.html), images, diagnostics, a list of relevant links, or [tables](https://azsupportdocs.azurewebsites.net/playbook/ApolloFAQFormatting.html#tables). 

:heavy_exclamation_mark: <span style="color:red">**Important**</span>:
An article that includes only links to other documents is not acceptable. 

### Recommended

<ul><li><a href="https://azsupportdocs.azurewebsites.net/elixir/articles/Diagnostics.html"><strong>Diagnostics</strong></a>: If you include one or more diagnostics, provide a brief diagnostic description that tells the user what each diagnostic does and how long it might take.</li>
	<ul><li><strong>Example</strong>: “This diagnostic is checking for network connectivity. It will take just a few minutes.”</li>
	</ul>
<li><strong>Clear, specific section headers</strong>. Generic headers like “Troubleshooting” or “Private endpoints” are not acceptable. Create a header specific to your section, or use one of the following examples:</li>
	<ul><li><strong>Examples</strong>: 
		<ul><li>“Common issues and solutions,”</li>
		<li>“Troubleshoot issues with [insert topic],”</li>
		<li>“FAQ: [insert topic],”</li>
		<li>“Step-by-step instructions to resolve [insert issue].” </li>
		</ul>
	</ul>
<li>A <strong><a href="https://azsupportdocs.azurewebsites.net/playbook/ApolloFAQLinks.html#links-in-the-resources-section">Resources</a></strong> section (if applicable) with additional links.</li>
	<ul><li>No more than 5 links total and only links not mentioned in the article.</li> 
	<li>Explanatory phrases added for links only if necessary.</li>
	</ul>
<li>Include <a href="https://azsupportdocs.azurewebsites.net/elixir/articles/Azurekb.html"><strong>AzureKB</strong></a> to provide dynamic Bing-powered search results at the end of the article. AzureKB adds an average of +1pp ShS and requires no additional effort.</li>
	<ul><li><strong>Note</strong>: Bonsai will eventually flag articles without AzureKB and recommend adding AzureKB. It’s best practice to include AzureKB in your original article. 
	<li>To include AzureKB, use the following H3 heading and schema:</li>
	</ul>
</ul>

        ### Relevant results from the web
		
		<azureKB>
			<client>portal</client>
		</azureKB>	

### Additional guidance

* **After committing, check for validation errors** like: 
  * Blocking errors (such as errors in metadata or broken links) ![error image](https://github.com/MadMadrox/portfolio/blob/main/July23/images/ApolloError.png) 
  * Non-blocking warnings (such as potential spelling errors) ![warning image](https://github.com/MadMadrox/portfolio/blob/main/July23/images/ApolloWarning.png)
* **For longer articles, use headings (level 3 headers) or** [collapsible sections](https://azsupportdocs.azurewebsites.net/elixir/articles/AccordionSections.html) to guide the customer, including descriptive titles for each heading or section.
* **Under each heading or within each collapsible section, format subheadings in bold font** if subsections (such as individual solutions) exceed a total of 5, or if subsections are complex.
* **Add rich components** such as videos or images to enhance the customer experience.
* Use [**tables**](https://azsupportdocs.azurewebsites.net/playbook/ApolloFAQFormatting.html#tables) as a scannable alternative for long lists of solutions or other complex elements.

## Review exceptions
:heavy_exclamation_mark: <span style="color:red">**Important**</span>: **When submitting a review exception, make sure to notify the editors!** 

### Expedited review - Minimum requirements fulfilled
For an expedited review, be sure to state the business reason for the expedited review in your notification to the editors (see above). Editors review PRs with a two-day SLA prioritizing the oldest PRs first, so diverging from this requires clear justification.

### Small changes - Minimum requirements deferment
If you submit a revised article with small changes only (see definition below), editors will defer the minimum requirements and publish the article with no further changes. As a courtesy, they’ll also do a full review following Apollo guidelines, and will follow up with a reminder for you to make the necessary content edits later.

To notify the editors, add a hidden comment to your file/article. 
- Insert the following HTML syntax on the **bottom line** of the article and adjust the (Date) to date of submission : `<! –- (Date) SmallChange -->.`

**Small changes** include:
<ul><li>Metadata updates
	</li><li>Link additions or deletions; link text updates or broken link updates 
	</li><li>Code block revisions within the article 
	</li><li>Diagnostic additions 
	</li><li>Fulfilling Elixir (Bonsai) recommendations
</li></ul>
