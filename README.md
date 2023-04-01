# Format

To contribute to our docs, you must follow the format below.

    ---
    id: <id>
    title: <title>
    description: <description>
    keywords: <keywords>
    ---
   Please note that `description` and `keywords` are **not required**, but we encourage you to use these for SEO purposes.
   

## Example #1
Using `description` and `keywords`.

```
---
id: my-doc-page
title: My Doc Page
description: This is my fancy doc page!
keywords: my,doc,page
---
```

## Example #2
Without `description` and `keywords`.

```
---
id: my-doc-page
title: My Doc Page
---
```

# Sidebar
After creating a page, you'll need to add it in `sidebar.js`, under an existing or new category. All category folders and doc files are stored in `/docs/`.

## Using an existing category
Adding your page to an existing category is a case of just adding one line. See the example below.
```
{
	type: 'category',
	label: 'Category #1',
	collapsible: true,
	collapsed: true,
	items: [
		'category-1/doc-1',
		'category-1/doc-b',
		'category-1/doc-c',
		'folder-name/your-file',
	],
},
```
To keep our directory clean and tidy, please ensure your file is under the relevant category folder in the `/docs/` directory. **You do not need to add `.md` to the end of your entry.**

## Using a new category
If existing categories are not relevant, you can add a new category using the example below.
```
{
	type: 'category',
	label: 'Category Name',
	collapsible: true,
	collapsed: true,
	items: [
		'folder-name/your-file',
	],
},
```
Please ensure you have created a new folder in `/docs/` and stored your new file inside. The folder name should correspond with the `label` you have set above, for ease of reference. **You do not need to add `.md` to the end of your entry.**

# Support
If you have any problems, please reach out to us on our [**Discord**](https://discord.gg/Aqzwbng4mc). Only open GitHub issues for **technical-related problems**.

