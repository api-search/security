---
api_key_in: []
api_specs:
- filename: quenza-archiveclient-api-openapi.yml
  format: yaml
  label: Quenza ArchiveClient API
  slug: quenza-archiveclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-archiveclient-api-openapi.yml
- filename: quenza-attachgroupmembers-api-openapi.yml
  format: yaml
  label: Quenza AttachGroupMembers API
  slug: quenza-attachgroupmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-attachgroupmembers-api-openapi.yml
- filename: quenza-clients-api-openapi.yml
  format: yaml
  label: Quenza Clients API
  slug: quenza-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-clients-api-openapi.yml
- filename: quenza-createclient-api-openapi.yml
  format: yaml
  label: Quenza CreateClient API
  slug: quenza-createclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-createclient-api-openapi.yml
- filename: quenza-creategroup-api-openapi.yml
  format: yaml
  label: Quenza CreateGroup API
  slug: quenza-creategroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-creategroup-api-openapi.yml
- filename: quenza-createmember-api-openapi.yml
  format: yaml
  label: Quenza CreateMember API
  slug: quenza-createmember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-createmember-api-openapi.yml
- filename: quenza-groups-api-openapi.yml
  format: yaml
  label: Quenza Groups API
  slug: quenza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-groups-api-openapi.yml
- filename: quenza-listclient-api-openapi.yml
  format: yaml
  label: Quenza ListClient API
  slug: quenza-listclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listclient-api-openapi.yml
- filename: quenza-listmember-api-openapi.yml
  format: yaml
  label: Quenza ListMember API
  slug: quenza-listmember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listmember-api-openapi.yml
- filename: quenza-listtask-api-openapi.yml
  format: yaml
  label: Quenza ListTask API
  slug: quenza-listtask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listtask-api-openapi.yml
- filename: quenza-members-api-openapi.yml
  format: yaml
  label: Quenza Members API
  slug: quenza-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-members-api-openapi.yml
- filename: quenza-showclient-api-openapi.yml
  format: yaml
  label: Quenza ShowClient API
  slug: quenza-showclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-showclient-api-openapi.yml
- filename: quenza-tasks-api-openapi.yml
  format: yaml
  label: Quenza Tasks API
  slug: quenza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-tasks-api-openapi.yml
- filename: quenza-unarchiveclient-api-openapi.yml
  format: yaml
  label: Quenza UnarchiveClient API
  slug: quenza-unarchiveclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-unarchiveclient-api-openapi.yml
- filename: quenza-updateclient-api-openapi.yml
  format: yaml
  label: Quenza UpdateClient API
  slug: quenza-updateclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-updateclient-api-openapi.yml
- filename: quenza-updatemember-api-openapi.yml
  format: yaml
  label: Quenza UpdateMember API
  slug: quenza-updatemember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-updatemember-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Quenza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quenza secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quenza
provider_slug: quenza
scheme_count: 1
schemes:
- description: 'Authenticate using a **Bearer token** in the `Authorization` header:


    ```

    Authorization: Bearer {your-token}

    ```


    You can generate or regenerate your API token in your Quenza workspace under

    **Settings → Developer Tools → API Token**.'
  name: http
  scheme: bearer
  sources:
  - openapi/quenza-openapi.yml
  type: http
slug: quenza-authentication
source_filename: quenza-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quenza-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  description: |-\n    Authenticate using a **Bearer token** in the `Authorization` header:\n\n    ```\n    Authorization: Bearer {your-token}\n    ```\n\n    You can generate or regenerate your API token in your Quenza workspace under\n    **Settings → Developer Tools → API Token**.\n  sources:\n  - openapi/quenza-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/authentication/quenza-authentication.yml
summary_line: http · 1 scheme
tags:
- Coaching
- Therapy
- Client Engagement
- Digital Health
- Mental Health
- Practice Management
- Positive Psychology
---
