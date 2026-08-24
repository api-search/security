---
api_key_in:
- unknown
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Insidesales Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: InsideSales (XANT / InsideSales.com) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: InsideSales (XANT / InsideSales.com)
provider_slug: insidesales-com
scheme_count: 1
schemes:
- in: unknown
  issuance:
    actor: Playbooks administrator
    note: Only administrators can create a key. The docs do not publish which HTTP header or query parameter carries the key — that detail lived only in the apiDoc.js reference at ci-global-api.pdlmpapis.insidesales.com/apidoc/, which no longer resolves (DNS SERVFAIL, probed 2026-08-23). The single Wayback capture of that reference (20210926063143) archived only the empty apiDoc shell; api_data.js was never captured, so the parameter name is not recoverable from any public source.
    path: Playbooks Manager App > Settings > Calls > Call Recording > ADD KEY
    self_service: false
  name: PlaybooksCallRecordingAccessKey
  parameter_name: unknown
  permission_model:
    minimum_permissions: 1
    mutable_after_creation: false
    note: '"Each key must have at least one permission to be created." Permissions cannot be changed once the key is made; only the key name can be renamed. Revocation is deletion — there is no published rotation or expiry mechanism, and no published key lifetime.'
    rename_allowed: true
    revocation: Delete the key from Playbooks Manager App > Settings > Calls > Call Recording.
  permissions:
  - grants: Retrieve a call recording by CDR ID.
    id: download-recordings
    label: Allow this key to download recordings
  - grants: Systematically start or stop recording on a live call.
    id: control-recordings
    label: Allow this key to start/pause recordings
  scope: Organization-wide. The docs warn "anyone who has access to the key will have access to your call recordings" — the key is not bound to a user, a rep, or a subset of recordings.
  sources:
  - https://helpcenter.insidesales.com/playbooks/call-recording-api/
  type: apiKey
slug: insidesales-com-authentication
source_filename: insidesales-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://helpcenter.insidesales.com/playbooks/call-recording-api/\ndocs: https://helpcenter.insidesales.com/playbooks/call-recording-api/\nnote: >-\n  Derived mechanically from OpenAPI was not possible — InsideSales publishes no machine-readable\n  contract (see conformance/insidesales-com-conformance.yml). This profile is read verbatim from the\n  company's own Call Recording API help article and the 9 July 2021 product update that introduced\n  the Call Recording Control API.\nsummary:\n  types: [apiKey]\n  api_key_in: [unknown]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: PlaybooksCallRecordingAccessKey\n  type: apiKey\n  in: unknown\n  parameter_name: unknown\n  sources: [https://helpcenter.insidesales.com/playbooks/call-recording-api/]\n  issuance:\n    self_service: false\n    actor: Playbooks administrator\n    path: Playbooks Manager App > Settings > Calls > Call Recording > ADD\
  \ KEY\n    note: >-\n      Only administrators can create a key. The docs do not publish which HTTP header or query\n      parameter carries the key — that detail lived only in the apiDoc.js reference at\n      ci-global-api.pdlmpapis.insidesales.com/apidoc/, which no longer resolves (DNS SERVFAIL,\n      probed 2026-08-23). The single Wayback capture of that reference (20210926063143) archived\n      only the empty apiDoc shell; api_data.js was never captured, so the parameter name is not\n      recoverable from any public source.\n  permissions:\n  - id: download-recordings\n    label: Allow this key to download recordings\n    grants: Retrieve a call recording by CDR ID.\n  - id: control-recordings\n    label: Allow this key to start/pause recordings\n    grants: Systematically start or stop recording on a live call.\n  permission_model:\n    minimum_permissions: 1\n    mutable_after_creation: false\n    rename_allowed: true\n    revocation: Delete the key from Playbooks Manager App\
  \ > Settings > Calls > Call Recording.\n    note: >-\n      \"Each key must have at least one permission to be created.\" Permissions cannot be changed once\n      the key is made; only the key name can be renamed. Revocation is deletion — there is no\n      published rotation or expiry mechanism, and no published key lifetime.\n  scope: >-\n    Organization-wide. The docs warn \"anyone who has access to the key will have access to your call\n    recordings\" — the key is not bound to a user, a rep, or a subset of recordings.\nresource_identifier:\n  name: CDR ID\n  full_name: Call Detail Record ID\n  description: >-\n    Unique identifier for each call placed within Playbooks. Read from the trailing id of the\n    Playbooks Call Recording field written back to the CRM, e.g.\n    https://callrecordings.insidesales.com?id=5858485\n  note: >-\n    For Salesforce tenants the Playbooks Call Recording field only exists if the Playbooks unmanaged\n    package is installed or the field is created\
  \ manually.\naccess_gate:\n  control_api: sales-gated\n  detail: >-\n    The 9 July 2021 product update that shipped the Call Recording Control API states plainly: \"To\n    begin using this feature please contact your Customer Success Manager.\" The download half of the\n    API is self-serve for an administrator; the start/stop control half is not.\n  source: https://helpcenter.insidesales.com/releases/july-9th-2021-product-update/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insidesales-com/refs/heads/main/authentication/insidesales-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Sales
- Sales Engagement
- Sales Automation
- CRM
- Call Recording
- Artificial Intelligence
- Salesforce
- Microsoft Dynamics
- Enterprise Software
---
