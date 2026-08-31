---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Olaris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Olaris declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Olaris
provider_slug: olaris
scheme_count: 2
schemes:
- applies_to: MCP session and read-only tools (tools/list, GetBusinessDetails, SearchInSite, SearchSiteApiDocs, BrowseWixRESTDocsMenu, ReadFullDocsArticle, ReadFullDocsMethodSchema)
  evidence: llms.txt states "No authentication required to connect to the MCP endpoint"; an anonymous POST tools/list on 2026-08-26 returned HTTP 200 with the full nine-tool manifest.
  name: none
  type: none
- applies_to: CallWixSiteAPI and ExecuteWixAPI (both require a visitorToken parameter)
  evidence: The tools/list inputSchema marks visitorToken as required on CallWixSiteAPI and ExecuteWixAPI; llms.txt states GenerateVisitorToken "must be called before making any CallWixSiteAPI request if no visitor token is already available in context."
  issued_by_tool: GenerateVisitorToken
  name: wix-visitor-token
  note: An anonymous visitor session, not an account credential. It authorizes actions on a visitor's behalf against public site data only.
  type: bearer-like session token
slug: olaris-authentication
source_filename: olaris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.myolaris.com/llms.txt\ndocs: https://dev.wix.com/docs/develop-websites/articles/get-started/about-the-wix-site-mcp\nscope: 'Olaris publishes no API and therefore no API authentication documentation.\n  This file records the auth model of the ONE callable machine surface on a host Olaris\n  controls — the Wix Site MCP endpoint at https://www.myolaris.com/_api/mcp — as stated\n  in Olaris'' own llms.txt and as observed on a live anonymous probe. It is a platform-provided\n  surface, not a first-party Olaris product API.'\nschemes:\n- name: none\n  type: none\n  applies_to: MCP session and read-only tools (tools/list, GetBusinessDetails, SearchInSite,\n    SearchSiteApiDocs, BrowseWixRESTDocsMenu, ReadFullDocsArticle, ReadFullDocsMethodSchema)\n  evidence: 'llms.txt states \"No authentication required to connect to the MCP endpoint\";\n    an anonymous POST tools/list on 2026-08-26 returned HTTP 200 with the full nine-tool\n\
  \    manifest.'\n- name: wix-visitor-token\n  type: bearer-like session token\n  applies_to: CallWixSiteAPI and ExecuteWixAPI (both require a visitorToken parameter)\n  issued_by_tool: GenerateVisitorToken\n  evidence: 'The tools/list inputSchema marks visitorToken as required on CallWixSiteAPI\n    and ExecuteWixAPI; llms.txt states GenerateVisitorToken \"must be called before\n    making any CallWixSiteAPI request if no visitor token is already available in\n    context.\"'\n  note: An anonymous visitor session, not an account credential. It authorizes actions\n    on a visitor's behalf against public site data only.\noauth: false\napi_keys: false\nmtls: false\nopenid_connect: false\ndata_boundary: 'Only public site content is reachable. No patient, clinical, laboratory\n  or myOLARIS-KTdx result data is exposed through this surface, and Olaris publishes\n  no authenticated clinical or ordering API — test ordering runs through Labcorp''s\n  existing physician portal, not an Olaris endpoint.'\n\
  x-evidence:\n- url: https://www.myolaris.com/llms.txt\n  status: 200\n- url: https://www.myolaris.com/_api/mcp\n  status: 200\n- url: https://www.myolaris.com/.well-known/oauth-authorization-server\n  status: 400\n- url: https://www.myolaris.com/.well-known/openid-configuration\n  status: 400\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olaris/refs/heads/main/authentication/olaris-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Healthcare
- Diagnostics
- Precision Medicine
- Metabolomics
- Machine-Learning
- Biomarkers
- Laboratory
- Transplant
- Life Sciences
---
