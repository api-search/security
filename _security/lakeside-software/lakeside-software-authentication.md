---
api_key_in: []
auth_types: []
description: SysTrack separates human sign-in from programmatic access. Interactive users authenticate to the SysTrack Cloud through Azure AD B2C / Microsoft Entra ID or via SAML SSO. Programmatic callers use scoped SysTrack API keys, issued per capability (Read, Read/Write, Ingest, SysTrack AI Partner). The SysTrack AI MCP Server additionally supports OAuth 2.0 with Microsoft Entra ID as of the 11.7.1.29 hotfix. No public OpenAPI is published, so this profile is harvested from documentation rather than derived from securitySchemes.
kind: authentication
layout: security
method: searched
name: Lakeside Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lakeside Software declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Lakeside Software
provider_slug: lakeside-software
scheme_count: 6
schemes:
- applies_to:
  - SysTrack API
  - Data API (legacy)
  description: The documented authentication method for the SysTrack API on cloud tenants. Keys are generated in the SysTrack tenant and presented on each request. Key variants named in the documentation are "SysTrack Read" and "SysTrack Read/Write".
  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1
  environments:
  - cloud
  id: systrack-api-key
  location: null
  location_note: The header/parameter name carrying the key is documented only inside the customer-gated API reference; not recorded here rather than guessed.
  name: SysTrack API key
  type: apiKey
  variants:
  - access: read-only
    name: SysTrack Read
  - access: read-write
    name: SysTrack Read/Write
- applies_to:
  - SysTrack Ingest API
  description: A valid Ingest API key is required for authentication to the Data Ingest endpoints.
  docs: https://documentation.lakesidesoftware.com/docs/ingest-api-user-guide
  environments:
  - cloud
  id: ingest-api-key
  name: Ingest API key
  type: apiKey
- applies_to:
  - SysTrack AI programmatic access
  - SysTrack DEX Analytics MCP Server
  description: Required, alongside the SysTrack AI add-on package, to use SysTrack AI programmatic access and the DEX Analytics MCP Server.
  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1
  environments:
  - cloud
  id: systrack-ai-partner-key
  name: SysTrack AI (Partner) key
  type: apiKey
- applies_to:
  - SysTrack AI MCP Server
  description: OAuth 2.0 authentication with Microsoft Entra ID was added for the SysTrack AI MCP Server.
  docs: https://documentation.lakesidesoftware.com/docs/whats-new-in-systrack
  id: entra-oauth2-mcp
  name: OAuth 2.0 with Microsoft Entra ID
  scopes_note: No public scope reference is published, so no scopes/ artifact was produced rather than inventing one.
  scopes_published: false
  since: 11.7.1.29 (May 2026)
  type: oauth2
- applies_to:
  - SysTrack API (on-premises / legacy method)
  description: The "Programmatic Access to SysTrack" course lists service account credentials as the access needed when using the legacy method, and covers authentication on on-premises installations separately from cloud tenants.
  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1
  environments:
  - on-premises
  id: service-account
  name: Service account credentials
  type: http
- description: Not a caller-authentication scheme — this is how a receiver verifies that a webhook came from SysTrack. HMAC-SHA256 over the raw request body, Base64-encoded, delivered in the x-lakeside-hmac-sha256 header.
  detail: asyncapi/lakeside-software-webhooks.yml
  direction: outbound
  docs: https://documentation.lakesidesoftware.com/docs/signed-secret-authentication-for-webhooks
  id: webhook-signed-secret
  name: Signed Secret (outbound webhook verification)
  type: hmac
slug: lakeside-software-authentication
source_filename: lakeside-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://documentation.lakesidesoftware.com/docs/systrack-api-1,\n  https://documentation.lakesidesoftware.com/docs/ingest-api-user-guide,\n  https://documentation.lakesidesoftware.com/docs/cloud-authentication-microsoft-entra-id,\n  https://documentation.lakesidesoftware.com/docs/systrack-versions-and-life-cycle,\n  https://documentation.lakesidesoftware.com/docs/whats-new-in-systrack\ndescription: >-\n  SysTrack separates human sign-in from programmatic access. Interactive users authenticate to the\n  SysTrack Cloud through Azure AD B2C / Microsoft Entra ID or via SAML SSO. Programmatic callers use\n  scoped SysTrack API keys, issued per capability (Read, Read/Write, Ingest, SysTrack AI Partner).\n  The SysTrack AI MCP Server additionally supports OAuth 2.0 with Microsoft Entra ID as of the\n  11.7.1.29 hotfix. No public OpenAPI is published, so this profile is harvested from documentation\n  rather than derived from\
  \ securitySchemes.\nderived_from_openapi: false\nderived_from_openapi_note: >-\n  Lakeside publishes no public OpenAPI/Swagger document — the API reference at\n  documentation.lakesidesoftware.com/apidocs sits behind customer sign-in (302 to\n  identity.document360.io). derive-authentication.py had no spec to read.\nschemes:\n- id: systrack-api-key\n  type: apiKey\n  name: SysTrack API key\n  applies_to: [SysTrack API, Data API (legacy)]\n  environments: [cloud]\n  description: >-\n    The documented authentication method for the SysTrack API on cloud tenants. Keys are generated\n    in the SysTrack tenant and presented on each request. Key variants named in the documentation\n    are \"SysTrack Read\" and \"SysTrack Read/Write\".\n  variants:\n  - name: SysTrack Read\n    access: read-only\n  - name: SysTrack Read/Write\n    access: read-write\n  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1\n  location: null\n  location_note: >-\n    The header/parameter name carrying\
  \ the key is documented only inside the customer-gated API\n    reference; not recorded here rather than guessed.\n- id: ingest-api-key\n  type: apiKey\n  name: Ingest API key\n  applies_to: [SysTrack Ingest API]\n  environments: [cloud]\n  description: A valid Ingest API key is required for authentication to the Data Ingest endpoints.\n  docs: https://documentation.lakesidesoftware.com/docs/ingest-api-user-guide\n- id: systrack-ai-partner-key\n  type: apiKey\n  name: SysTrack AI (Partner) key\n  applies_to: [SysTrack AI programmatic access, SysTrack DEX Analytics MCP Server]\n  environments: [cloud]\n  description: >-\n    Required, alongside the SysTrack AI add-on package, to use SysTrack AI programmatic access and\n    the DEX Analytics MCP Server.\n  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1\n- id: entra-oauth2-mcp\n  type: oauth2\n  name: OAuth 2.0 with Microsoft Entra ID\n  applies_to: [SysTrack AI MCP Server]\n  since: 11.7.1.29 (May 2026)\n  description:\
  \ >-\n    OAuth 2.0 authentication with Microsoft Entra ID was added for the SysTrack AI MCP Server.\n  scopes_published: false\n  scopes_note: >-\n    No public scope reference is published, so no scopes/ artifact was produced rather than\n    inventing one.\n  docs: https://documentation.lakesidesoftware.com/docs/whats-new-in-systrack\n- id: service-account\n  type: http\n  name: Service account credentials\n  applies_to: [SysTrack API (on-premises / legacy method)]\n  environments: [on-premises]\n  description: >-\n    The \"Programmatic Access to SysTrack\" course lists service account credentials as the access\n    needed when using the legacy method, and covers authentication on on-premises installations\n    separately from cloud tenants.\n  docs: https://documentation.lakesidesoftware.com/docs/systrack-api-1\n- id: webhook-signed-secret\n  type: hmac\n  name: Signed Secret (outbound webhook verification)\n  direction: outbound\n  description: >-\n    Not a caller-authentication\
  \ scheme — this is how a receiver verifies that a webhook came from\n    SysTrack. HMAC-SHA256 over the raw request body, Base64-encoded, delivered in the\n    x-lakeside-hmac-sha256 header.\n  detail: asyncapi/lakeside-software-webhooks.yml\n  docs: https://documentation.lakesidesoftware.com/docs/signed-secret-authentication-for-webhooks\nuser_authentication:\n  description: Interactive sign-in to the SysTrack Cloud console (not API authentication).\n  methods:\n  - name: Azure AD B2C / Microsoft Entra ID\n    application_name: SysTrack Cloud Edition\n    application_id: 3bc280a0-0206-4276-acf1-b7ee6a7f5b66\n    permission_requested: User.Read\n    data_read: First name, last name, and email address only\n    admin_consent_required: true\n    docs: https://documentation.lakesidesoftware.com/docs/cloud-authentication-microsoft-entra-id\n  - name: SAML SSO\n    docs: https://documentation.lakesidesoftware.com/docs/configure-sso-saml\nauthorization:\n  user_to_system:\n    description: >-\n\
  \      User-to-System Authorization for SysTrack AI end-user channels was introduced in the 11.7.1.22\n      hotfix, constraining which systems a given end user may act against through AI channels.\n    since: 11.7.1.22 (May 2026)\n    source: https://documentation.lakesidesoftware.com/docs/whats-new-in-systrack\nfair_use:\n  documented: true\n  detail_public: false\n  note: >-\n    The SysTrack API course outline includes a \"Fair Use Policy\" section, indicating usage limits\n    exist, but the policy text is inside the customer-gated course. No public rate-limit numbers\n    were found.\n  source: https://documentation.lakesidesoftware.com/docs/systrack-api-1\naudit:\n  description: >-\n    SysTrack exposes an Audit API for reading the audit trail, and logs SysTrack AI automation\n    execution activity for auditing.\n  source: https://documentation.lakesidesoftware.com/docs/systrack-api-1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakeside-software/refs/heads/main/authentication/lakeside-software-authentication.yml
summary_line: 6 schemes
tags:
- Company
- Digital Employee Experience
- Endpoint Monitoring
- IT Operations
- Observability
- Device Management
- End User Computing
- Analytics
- Virtual Desktop
- ITSM
---
