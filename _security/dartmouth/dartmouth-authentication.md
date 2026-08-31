---
api_key_in: []
api_specs:
- filename: dartmouth-class-search-api-openapi.yml
  format: yaml
  label: Dartmouth Class Search API
  slug: class-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dartmouth/refs/heads/main/openapi/dartmouth-class-search-api-openapi.yml
auth_types: []
description: How Dartmouth's institution-operated interfaces authenticate. Every row was established by calling the surface, not by reading a claim about it.
kind: authentication
layout: security
method: probed
name: Dartmouth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dartmouth College declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Dartmouth College
provider_slug: dartmouth
scheme_count: 0
schemes: []
slug: dartmouth-authentication
source_filename: dartmouth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live HTTP probes of api.dartmouth.edu, chat.dartmouth.edu, developer.dartmouth.edu, courses.dartmouth.edu\nprovider: Dartmouth College\nproviderId: dartmouth\ndescription: >-\n  How Dartmouth's institution-operated interfaces authenticate. Every row was\n  established by calling the surface, not by reading a claim about it.\nsurfaces:\n  - name: Dartmouth Class Search API\n    host: courses.dartmouth.edu\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Keyless and unauthenticated. A POST with no credentials returns a full page of\n      class sections (HTTP 200, 1393 sections for term 202609 on 2026-08-30). The only\n      genuinely open programmable surface Dartmouth operates that this profile found.\n  - name: DartAPI\n    host: api.dartmouth.edu\n    x-operator: institution\n    scheme: http\n    bearerFormat: JWT\n    detail: >-\n      Every resource path returns {\"message\":\"Unauthorized\"} with HTTP\
  \ 401 to an\n      unauthenticated caller (/api/people/, /api/nextgen/class_schedules/, /api/ai/).\n      A JWT is minted by exchanging a manually issued API key at POST\n      https://api.dartmouth.edu/api/jwt — a GET on that path returns 405 Method Not\n      Allowed, confirming the endpoint exists and is POST-only. The API key itself is\n      issued by hand through the Dartmouth Help Desk against a Dartmouth Service Account.\n  - name: Dartmouth Chat AI API\n    host: chat.dartmouth.edu\n    x-operator: institution\n    scheme: http\n    bearerFormat: API key\n    detail: >-\n      /api/models and /api/v1/models return {\"detail\":\"Not authenticated\"} with HTTP 401.\n      Requires DARTMOUTH_API_KEY. Affiliation-gated; not self-service.\n  - name: DartAPI developer portal\n    host: developer.dartmouth.edu\n    x-operator: institution\n    scheme: saml\n    detail: >-\n      The portal, including its /docs/ pages, 302s to Microsoft Entra ID SAML2 at\n      login.microsoftonline.com\
  \ (tenant 995b0936-48d6-40e5-a31e-bf689ec9446f). No\n      documentation page is readable without a Dartmouth NetID, so the API reference\n      cannot be verified from outside the institution.\n  - name: Institutional SSO / identity federation\n    host: login.dartmouth.edu, login2.dartmouth.edu\n    x-operator: institution\n    scheme: saml\n    detail: >-\n      Apereo CAS fronting Microsoft Entra ID for interactive login, and publishing\n      SAML2/SAML1.1 IdP metadata into InCommon as urn:mace:incommon:dartmouth.edu.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dartmouth/refs/heads/main/authentication/dartmouth-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Private Research University
- Course Catalog
- Identity Federation
- Research Data
- Open Data
- Artificial Intelligence
---
