---
api_key_in: []
api_specs:
- filename: university-of-twente-energy-api-openapi.yml
  format: yaml
  label: University of Twente Energy API
  slug: energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-twente/refs/heads/main/openapi/university-of-twente-energy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Twente Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Twente declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Twente
provider_slug: university-of-twente
scheme_count: 0
schemes: []
slug: university-of-twente-authentication
source_filename: university-of-twente-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: openapi/_original/university-of-twente-energy-api-openapi.json\nx-operator: institution\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The University of Twente Energy API is fully public. The harvested OpenAPI declares no\n    components.securitySchemes and no top-level or per-operation security requirement, and a\n    live unauthenticated GET to https://energyapi.utwente.nl/api/Energy returned 200 with real\n    campus data on 2026-09-01. There is no key to request, no registration, no account and no\n    quota gate. Absence of authentication here is a deliberate open-data posture, not an\n    omission: the university's own open-data page states the platform \"opens all energy-related\n    data up to the public\".\nschemes: []\nobserved:\n- surface: https://energyapi.utwente.nl/api/Energy\n  probed: '2026-09-01'\n  status: 200\n  credential_sent: none\n  result: 200 with the full 103-resource list;\
  \ no WWW-Authenticate, no 401, no 403.\n- surface: https://energyapi.utwente.nl/api/Energy/universiteit-twente/electricity\n  probed: '2026-09-01'\n  status: 200\n  credential_sent: none\n  result: 200 with metered kWh series; no credential required.\ninstitutional_authentication_elsewhere:\n  note: >-\n    Authentication at the University of Twente is not absent — it is simply not on the open data\n    API. The university operates its own SAML 2.0 identity provider, federated through SURFconext,\n    and every gated institutional surface sits behind it. This is recorded as a federation surface\n    in apis.yml, not as an authentication scheme of the Energy API.\n  identity_provider:\n    protocol: SAML 2.0\n    entity_id: https://sts.windows.net/723246a1-c3f5-43c5-acdc-43adb404ac4d/\n    platform: Microsoft Entra ID (tenant region EU)\n    shibboleth_scope: utwente.nl\n    federation: SURFconext (Dutch national research and education federation)\n    federation_metadata: https://metadata.surfconext.nl/idps-metadata.xml\n\
  \    tenant_metadata: https://login.microsoftonline.com/723246a1-c3f5-43c5-acdc-43adb404ac4d/federationmetadata/2007-06/federationmetadata.xml\n    oidc_discovery: https://login.microsoftonline.com/723246a1-c3f5-43c5-acdc-43adb404ac4d/v2.0/.well-known/openid-configuration\n    oidc_scopes_supported: [ openid, profile, email, offline_access ]\n    probed: '2026-09-01'\n    evidence: >-\n      The SURFconext IdP metadata aggregate carries an EntityDescriptor for this entityID with\n      mdui:DisplayName \"University of Twente\" / \"Universiteit Twente\", md:OrganizationURL\n      http://www.utwente.nl/ and shibmd:Scope regexp=\"false\" utwente.nl. The same tenant GUID\n      appears independently in the canvas.utwente.nl login redirect and in the ctid parameter of\n      the Power BI report embedded on the university's own open-data page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-twente/refs/heads/main/authentication/university-of-twente-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Technical University
- Netherlands
- Europe
- Open Data
- Energy
- Sustainability
- Research Data
- Identity Federation
- Student Mobility
- Open Science
---
