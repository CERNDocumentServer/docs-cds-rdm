# Reference

## REST APIs

CDS Repository exposes a REST API that allows you to programmatically interact with records, files, communities, and more. It follows the [InvenioRDM REST API](https://inveniordm.docs.cern.ch/reference/rest_api_index/) specification.

**Base URL:** `https://repository.cern/api/`

### Available resources

| Resource | Endpoint | Description |
|---|---|---|
| Records (list) | `/api/records` | Search and retrieve published records |
| Records (single) | `/api/records/{record_id}` | Retrieve a specific published record |
| Drafts | `/api/records/{draft_id}/draft` | Retrieve a draft record |
| Record files | `/api/records/{record_id}/files` | Retrieve files on a published record |
| Draft files | `/api/records/{draft_id}/draft/files` | Retrieve files on a draft record |
| Communities (list) | `/api/communities` | Search and retrieve communities |
| Communities (single) | `/api/communities/{community_id}` | Retrieve a specific community |
| OAI-PMH Sets | `/api/oaipmh/sets` | List OAI-PMH sets for metadata harvesting |
| Vocabularies | `/api/vocabularies/{type}` | Controlled vocabularies (e.g. `resourcetypes`, `experiments`, `licenses`) |

### Quick example

The following example retrieves the metadata for a published record:

```bash
curl https://repository.cern/api/records/<record_id>
```

To get a pretty-printed JSON response when exploring the API in a browser, append `?prettyprint=1` to the URL.

### Full API specification

The complete OpenAPI specification for the InvenioRDM REST API is available at:

- [Interactive API explorer](https://inveniosoftware.github.io/invenio-openapi/) — browse all endpoints, parameters, and response schemas.
- [InvenioRDM REST API reference](https://inveniordm.docs.cern.ch/reference/rest_api_index/) — narrative documentation with examples.

### Contact support

Some API endpoints or operations may require an authorisation token (e.g. accessing restricted records or performing write operations). If you need a token or have questions about API access, please contact the [CDS support team](https://cern.service-now.com/service-portal?id=service_element&name=CDS-Service).
