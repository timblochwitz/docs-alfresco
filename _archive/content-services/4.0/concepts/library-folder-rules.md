---
author: [Alfresco Documentation, Alfresco Documentation]
audience: 
category: 
option: 
---

# Automating repetitive tasks

In the library you can define folder rules to manage your content automatically. You can come up with many creative solutions to make sure specific content is moved or transformed \(or both!\) all without you having to do the work yourself.

There are three parts to a content rule:

-   The event that triggers the rule
-   The conditions the content has to meet
-   The action performed on the content

The events that can trigger a rule are:

-   A content item arrives in the folder
-   A content item leaves the folder \(it's moved or deleted\)
-   A content item in the folder is modified

Here are some examples of how you can use rules to automate repetitive tasks:

-   All content items placed in the *Drafts* folder are versioned
-   All content items placed in the *Drafts* folder become part of a simple workflow
-   All presentation documents placed in the *Published* folder will be transformed to Flash and copied to the *Assets* folder

-   **[Defining rules for a folder](../tasks/library-folder-rules-define.md)**  

-   **[Managing rules](../tasks/library-folder-rules-manage.md)**  
For a folder with rules, use the **Manage Rules** action to view and maintain the rule set.
-   **[Available transform options](../references/valid-tranformations.md)**  
There are many file types available in Alfresco and it's not always possible to transform one file type to another.
-   **[Creating a simple workflow](../tasks/library-folder-rules-simpleworkflow.md)**  
A workflow is a work procedure where workflow steps represent the activities users must follow in order to achieve the desired outcome. Simple workflow is generated by a folder that has a defined workflow rule. The rule dictates how the content entering, leaving, or currently residing in the folder is managed.

**Parent topic:**[Working with folders](../concepts/library-folder-intro.md)
