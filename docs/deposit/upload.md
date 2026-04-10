# Upload

To upload new content, first log in with your CERN account by clicking the login button in the top-right corner of any page.

![Login screen showing the CERN login button](images/login.jpg){ width="300" }

!!! Tip

    Only CERN and federated (EduGAIN) accounts can log in to CDS.

The easiest way to start a new upload is to first choose the community where you want to deposit the item. Read more about communities [here](../communities/communities.md).

You can view the communities you manage or search for other communities from the **Communities** menu in the top header:

![Communities menu listing communities you manage](images/communities.jpg)

Then click the green **New upload** button:

![Create a new upload for a community](images/communities-new-upload.jpg){ width="600" }

You will then see the deposit form:

![Deposit form showing metadata and file upload areas](images/deposit.jpg)

## Files

Click the **Upload files** button, or drag-and-drop one or more files onto the drop zone to start uploading.
By default you can upload up to 100 files with a combined maximum size of 50 GB.
If you need more, please contact us.

!!! Warning

    Make sure you have uploaded all your files before publishing. After publishing you cannot change the files.

![Files upload area in the deposit form](images/deposit-upload.jpg)

### File previewers

CDS can display many file types directly in the browser on the record's landing page, without requiring a download. The following formats are supported:

| Format | Examples |
|---|---|
| Images | JPG, PNG, GIF, TIFF, WebP |
| Documents | PDF |
| Plain text and code | TXT, CSV, JSON, XML, Markdown |
| Notebooks | Jupyter (`.ipynb`) |
| 3D models | GLTF, GLB |
| Archives | ZIP, WARC, TAR |

Files that are not in a supported format will show a download button instead of a preview.

![Jupyter notebook previewer](images/ipynb-preview.jpg)

![3D model previewer](images/gltf-preview.jpg)


!!! tip

    For 3D models, the previewer allows you to rotate, zoom, and pan the model directly in the browser. No additional software is required.

### Embargo

You can apply an embargo to one or more files by selecting **Apply an embargo** and configuring the embargo policy:

![Embargo options in the deposit form](images/deposit-embargo.jpg){ width="300" }

## Required metadata

The following fields are mandatory for each upload:

- **Title**: The title of your upload.
- **Resource type**: Choose one of the available resource types. If you are unsure which type to select, please [contact us](../index.md#need-help).
- **Author/Creators**: Add all authors or creators. Use the autocomplete field to search names; CDS synchronises with the [ORCID](https://orcid.org) and CERN user databases.

![Add authors using the autocomplete field](images/deposit-author.jpg){ width="600" }

## DOIs

If you need a DOI, select `No, I need one` and CDS will register a DOI automatically when the record is published. You can also reserve a DOI immediately using the **Get a DOI now!** button.

![Reserve or request a DOI](images/DOI_I_need.jpg)

If you already have an external DOI, provide it in the DOI field:

![Provide an existing DOI](images/DOI_external.jpg)

Avoid registering multiple DOIs for the same upload; if an external DOI already exists, use that one.

Because metadata is submitted to DataCite when registering a DOI, you cannot request a DOI for uploads that are fully restricted.

!!! tip

    When requesting a DOI, CDS will register two DOIs. Read more in the [DOI versioning FAQ](https://repository.cern/help/versioning).

## Related identifiers

If your record is related to another resource — for example, a preprint that has since been published in a journal, or a dataset associated with a paper — you should link them using **Related identifiers** in the deposit form. This improves discoverability and helps readers find all versions of a work.

Common relationships to declare:

| Situation | Relation type to use |
|---|---|
| This record is a preprint; a published version exists elsewhere | `IsVersionOf` (this record) → journal DOI |
| This record is the published version; a preprint exists | `HasVersion` (this record) → preprint DOI |
| A new version of this record exists | `IsPreviousVersionOf` → new version DOI |
| This record supersedes an older version | `IsNewVersionOf` → old version DOI |
| This record is a dataset used by a paper | `IsSupplementTo` → paper DOI |

To add a related identifier, open the deposit form, scroll to the **Related works** section, and enter the identifier (DOI, arXiv ID, handle, etc.) along with the appropriate relation type.

![Related identifiers](./images/related-identifiers.jpg)

For a full list of supported relation types and detailed guidance, see the [DataCite documentation on connecting related works](https://support.datacite.org/docs/connecting-to-works).

## Other metadata fields

The deposit form supports many additional metadata fields to help describe your upload. Common fields include:

- **Licenses and Copyright**: Specify license and copyright information for your upload.
- **CERN fields**: Add CERN-specific metadata such as experiment, accelerator, department, or project identifiers when applicable.
- **Publishing**: Publication details and related options.

## Access

See the [Access & Share](access-share.md) page for details on changing access restrictions and sharing settings.

## Preview, Save and Publish

You can preview or save your upload at any time using the **Preview** and **Save** buttons:

![Preview and Save buttons in the deposit form](images/deposit-actions.jpg){ width="300" }

When you are ready, publish your upload by clicking the **Publish** button. You will be asked to agree to the CDS terms and conditions, content policy, and Operational Circular 6.

![Publish the deposit to make it public](images/deposit-publish.jpg){ width="500" }

!!! Tip

    After publishing, you cannot change files, but you can update metadata at any time.
