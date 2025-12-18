# Commenting

On CDS, reviews are represented as a "request" to include a record in a given community.
These requests come with an advanced conversation feature, allowing everyone involved to discuss the submission in detail directly in CDS, without having to resort to an external communication tool.

This page showcases some of these features and explains how to use them.

## Writing a comment

![Example of a new comment being created in the rich text editor](./images/new_comment.png)

The text editor at the bottom of the page allows you to create a new comment.
This is a feature-rich editor with support for many advanced types of content.
The majority of content is edited in a "what you see is what you get" manner, where the contents of the editor clearly reflect how the comment will look once it is submitted.
However, there are some exceptions as explained below.

### LaTeX equations

<!-- TODO: update if/when we change the delimiter sign (see https://mattermost.web.cern.ch/it-dep/pl/yg6u9zk3rfnxdcyim5ebrpnfdw) -->

By surrounding LaTeX content with '`$`' you can ensure it's rendered as a mathematical equation.
The content is not rendered immediately in the editor.
However, you can preview it before submitting by clicking the "Preview math equations" button: 

![Math equation preview button](./images/preview_math_equation.png)

This will show the full comment in a dialog box, exactly as it will be shown to readers.
It will **not** save or submit the comment; it's just a temporary preview.
Once the comment is submitted, the equations will be shown fully-rendered as expected.

All **math-mode TeX/LaTeX** features supported by the web-based MathJax rendering engine can be used.
Keep in mind that text-mode macros and all types of environments are not supported.
You may also encounter [some other differences to normal TeX](https://docs.mathjax.org/en/latest/input/tex/differences.html).

### File attachments

<!-- TODO -->

### Quoting other comments

When writing a [reply to a comment](#replying-to-comments), you can include a "quote" of either all or part of the text.
You can also include multiple separate quotes if you want to reply to different sections of the text individually.

To quote the full comment, simply click the action menu (the 3 horizontal dots) on the comment you want to quote, and select "Quote reply":

![The dropdown action menu with the "quote reply" button an a sample comment](./images/quote_reply_dropdown.png)

Alternatively, to quote a part of a comment, highlight the text you wish to quote and click "Quote reply" in the popover that appears:

![The popover with the "quote reply" button above a highlighted piece of text](./images/quote_reply_popover.png)

Clicking this repeatedly will append the selected text to your reply comment.

### Auto-saved drafts

CDS saves your new comment draft automatically as you type.
The draft is saved locally in your browser and is **not** synchronised to your account.
This means your draft will not show up on a different device or browser.
It can also be lost if you're using a browser on a temporary kiosk computer or if you clear your browser's storage.
Your draft is restored automatically when you load the page if one can be found.

Separate drafts are stored for new comments and for any reply you're writing to an existing comment.
In-progress edits to existing comments are not saved.

!!! Warning
    Don't rely on auto-saving for storing drafts of long comments over an extended period of time.
    Browser storage can be volatile, and your draft can be lost at any time.
    This feature is solely intended to help recover recent drafts, e.g. in the case of accidentally reloading the page.

## Replying to a comment

To better preserve context, we recommend replying directly to comments through the "Write a reply" box instead of simply writing a new comment at the bottom of the page.
This helps group related information together and makes the review more readable.

To write a reply, simply click the "Write a reply" box.
When clicked, the full rich text editor will appear, and you can use all the same editing tools to compose the reply.

![The input to reply to a comment](./images/reply.png)

## Sharing a link to a comment

When dealing with requests that have a particularly large number of comments, it can be useful to share a link to a specific comment rather than the entire request.
By using a "deep link", you can guarantee that the recipient will always be taken to the exact comment you intended and that it will be clearly highlighted to them.

To copy a deep link to a comment, click the action menu (the 3 horizontal dots) and select "Copy link":

![The dropdown action menu with the "copy link" button](./images/copy_link.png)

The link will be automatically copied to your clipboard, ready for you to paste into a message or an email.
Unauthenticated users cannot necessarily open the link; it's important that the recipient has access to the request.
For example, they must be a member of the community or the submitter of the record.
Copying a link does not change the access restrictions of the request.

## Editing or deleting a comment

To edit a comment or reply, simply click the action menu (the 3 horizontal dots) and select "Edit".
The same rich text editor will appear as the one use to write new comments and replies.
Make your changes, and click the "Save" button.
Your changes will be applied immediately, and the comment will be marked with a small "Edited" label visible to all users.

To delete a comment or reply, select "Delete" from the action menu, then confirm your action by clicking "Delete" again in the dialog.
The comment will be deleted immediately, and replaced with a "stub".
Existing replies will **not** be deleted and new replies can still be added.
A deep link to the stub can still be copied, and existing deep links to the deleted comment will continue to work.

![An example of a deleted "stub" comment](./images/deleted_comment.png)

!!! Warning
    You cannot restore the original comment.
    The content is **deleted permanently**.

## Locking the conversation

In some cases, you may wish to lock the conversation after a certain period of the review is concluded.
Locking a conversation has the following effects:

- New comments cannot be created by anyone, including community curators
- Existing comments cannot be edited
- Existing comments can still be deleted
<!-- This is a CDS-specific feature, we should remove it when copying this over to generic docs -->
- Replying to existing comments is still allowed (replies can be created and deleted but not edited)

Community curators (and above) can unlock the conversation at any time.

To lock a conversation, click the "Lock conversation" button in the right-hand sidebar:

![The bottom part of the sidebar with the "Lock conversation" button visible](./images/lock_conversation.png)

To unlock, click the "Unlock conversation" button.

Locking and unlocking create an event visible to all viewers in the conversation timeline:

![The "lock"/"unlock" events in the timeline](./images/locking_event.png)
