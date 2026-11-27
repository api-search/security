---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ArchiCollab Authentication
name_suffix: Authentication
oauth_flows: []
overview: ArchiCollab declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ArchiCollab
provider_slug: collab-archi
scheme_count: 2
schemes:
- description: Personal API key created by an agency member under Réglages → Intégrations; acts with exactly the creator's rights, read-only by default, with optional "Autoriser l'écriture" and "Autoriser la publication au client" flags fixed at creation. Shown once; only a hash is stored. Lifetime chosen at creation (90 days suggested, or "Jamais"). Up to ten keys per person. Access is re-checked on every call, so a key stops working the moment membership is removed.
  header: x-api-key
  in: header
  name: apiKey
  quote: Le plafond est de 120 requêtes par minute et par clé.
  surface: REST API (https://collab.archi/api/v1)
  type: apiKey
- description: The MCP connector uses Streamable HTTP and OAuth 2.1; the user signs in to ArchiCollab and approves an authorization screen naming the assistant, with a separate unchecked box to allow writing on the user's behalf. Access is revocable.
  docs: https://collab.archi/help/guides/integrations/assistant-ia
  name: oauth2-mcp
  surface: MCP server (https://collab.archi/api/mcp)
  type: oauth2
slug: collab-archi-authentication
source_filename: collab-archi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://collab.archi/help/guides/integrations/cles-api\ndocs: https://collab.archi/help/guides/integrations/cles-api\nname: ArchiCollab authentication\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  surface: REST API (https://collab.archi/api/v1)\n  description: Personal API key created by an agency member under Réglages → Intégrations; acts with exactly the creator's rights, read-only by default, with optional \"Autoriser l'écriture\" and \"Autoriser la publication au client\" flags fixed at creation. Shown once; only a hash is stored. Lifetime chosen at creation (90 days suggested, or \"Jamais\"). Up to ten keys per person. Access is re-checked on every call, so a key stops working the moment membership is removed.\n  quote: \"Le plafond est de 120 requêtes par minute et par clé.\"\n- name: oauth2-mcp\n  type: oauth2\n  surface: MCP server (https://collab.archi/api/mcp)\n  description: The\
  \ MCP connector uses Streamable HTTP and OAuth 2.1; the user signs in to ArchiCollab and approves an authorization screen naming the assistant, with a separate unchecked box to allow writing on the user's behalf. Access is revocable.\n  docs: https://collab.archi/help/guides/integrations/assistant-ia\nnote: No OpenAPI is published (the API reference docs/api/README.md is not public), so this profile is read from the help-centre guides only. GET /api/v1/me reports what a key can see (organisation, role, project count, canWrite); it was not called.\n"
source_yaml_url: https://artifacts.apis.io/collab-archi/authentication/collab-archi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Architecture
- Collaboration
- PDF Annotation
- Construction
- Document Management
- MCP
- Software-as-a-Service
- France
---
