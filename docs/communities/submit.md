# Submit to a community

When you are uploading a record, you can submit it for review to a community. Communities may have their own metadata requirements and review workflows. This page explains what happens during submission, how to handle metadata issues, and how to manage community membership for your records.

## Where should I submit?

If you are unsure which community to submit to, the table below covers the most common cases:

| Your record | Recommended community |
|---|---|
| Publication, preprint, thesis, or conference paper authored at or in collaboration with CERN | [CERN Research](https://repository.cern/communities/cern-research) |
| Internal CERN report, note, or technical document | The relevant experiment or department community, if one exists |
| Dataset or software produced as part of a CERN experiment | The relevant experiment community |

You can always submit to more than one community if the record fits multiple scopes. See [Multiple communities](#multiple-communities) below.

!!! tip

    Start your upload from within a community by clicking **New upload** button on the community page. This pre-selects the community in the deposit form.

## Metadata checks

Before a record can be accepted into a community, CDS checks that the record's metadata meets the community's requirements. These checks run automatically when you submit.

![Metadata Check](./images/metadata_checks.png)

If any required fields are missing or invalid, you will see the list of issues that must be resolved before the submission can proceed as shown.

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

![Related identifiers](./images/related_identifiers.png)

For a full list of supported relation types and detailed guidance, see the [DataCite documentation on connecting related works](https://support.datacite.org/docs/connecting-to-works).

## Multiple communities

You can submit the same record to more than one community. Each submission is independent: a record can be accepted by one community while still under review in another.

To submit to an additional community after the record is already published:

1. Open the record's page.
2. Navigate to the Communities Panel (on computers, it's on the right; on phones/tablets, scroll down to the bottom of the page).
![Community Panel](./images/community_panel.png)

3. In the dropdown menu, select **Submit to community**.
4. Search for and select the community you want to submit to.
5. Add an optional message for the community curators and confirm the submission.

![Community Dialog Box](./images/community_dialog_box.png)

!!! note

    Each community has its own review process. Submitting to multiple communities means each community's curators will independently review and decide on your record.

## Removing from community

You can remove a record from a community if you no longer want it listed there, or if the community no longer fits the record's scope.

To remove a record from a community:

1. Open the record's page.
2. Navigate to the Communities Panel (on computers, it's on the right; on phones/tablets, scroll down to the bottom of the page).
3. In the dropdown menu, select **Manage communities**.
4. Click **Remove** and confirm the removal.

Removal is allowed in the following situations:

- The record has been accepted into the community and you are the record owner.
- The community curator removes the record from their community.
- A CDS administrator removes the record.

!!! warning

    Removing a record from a community does not delete the record itself. The record remains published and accessible via its DOI and direct URL. Only the community association is removed.

If a submission is still under review (not yet accepted), you can withdraw it instead of removing it:

1. Go to [your requests dashboard](https://repository.cern/me/requests), or click the inbox icon at the top right of any page.
2. Find the submission you wish to withdraw in the list of requests.
3. Click the **Cancel** button next to the relevant submission.

!!! tip

    If you open the individual request page, you'll also find a **Cancel** button in the top right corner for quick access.

---

## CERN Research

[**CERN Research**](https://repository.cern/communities/cern-research) is the one of the primary communities for storing scientific output produced at or in collaboration with CERN. It is intended for peer-reviewed publications, preprints, conference papers, theses, and other research outputs directly associated with CERN's scientific programme.

![CERN Research](./images/cern_research.png)

### Who should submit

You should submit to CERN Research if your record is:

- A publication or preprint authored by CERN staff, fellows, or associates.
- A thesis carried out at CERN or under CERN supervision.
- A conference contribution or proceedings paper from a CERN experiment or project.
- Any other research output that acknowledges CERN or is produced within a CERN experiment.

### Review workflow

Submissions to the CERN Research community go through a curator review before being listed in the community. The typical workflow is:

1. The CERN Research community curators receive a notification when you submit to review your submission.
2. If the metadata is complete and the record meets the community's scope, the curators accept the submission. The record then appears in the CERN Research community.
3. If changes are needed, the curators will leave a comment on the submission request. You will receive a notification and can update the record and ask for a re-review by dropping a comment.

!!! note

    Acceptance into CERN Research does not replace journal publication or any other formal publishing process. It makes the record discoverable within the CERN Research community on CDS.

## Submission policies

Before submitting to CDS, make sure your record complies with the relevant CERN policies:

- [**Operational Circular No. 6 (OC6)**](https://repository.cern/records/pnzz5-0b788) governs the dissemination of CERN publications. It defines which outputs must be deposited, embargo rules, and open-access obligations. All records submitted to CERN Research are expected to comply with OC6.
- The [**CERN Authors Guide**](https://cern-sis.github.io/cern-authors-guide/) provides practical guidance on authorship, affiliation formatting, acknowledgements, and how to handle journal submissions correctly. Following the guide helps ensure your record's metadata is accepted without changes during the review.
