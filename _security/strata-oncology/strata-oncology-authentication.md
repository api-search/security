---
api_key_in: []
api_specs:
- filename: strata-oncology-content-api-openapi.yml
  format: yaml
  label: Strata Oncology Website Content API
  slug: strata-oncology-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strata-oncology/refs/heads/main/openapi/strata-oncology-content-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Strata Oncology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strata Oncology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Strata Oncology
provider_slug: strata-oncology
scheme_count: 0
schemes: []
slug: strata-oncology-authentication
source_filename: strata-oncology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/strata-oncology-content-api-openapi.yml + live probes\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\nnote: >-\n  Strata Oncology publishes no API authentication documentation. The one public API surface - the WordPress\n  REST content API at https://strataoncology.com/wp-json - serves its read collections anonymously with no\n  credential of any kind, so its OpenAPI declares no securitySchemes. Because the provider does not document\n  an authentication model, no `Authentication` pointer is wired into apis.yml; this file records the observed\n  reality rather than asserting a documented auth posture.\nschemes: []\nobserved:\n- surface: Website content API\n  base_url: https://strataoncology.com/wp-json\n  authentication: none\n  evidence: >-\n    GET /wp/v2/pages, /wp/v2/publications, /wp/v2/resources, /wp/v2/team and /api/publications all returned\n    200 with no Authorization header on 2026-08-02.\n\
  \  privileged_routes: >-\n    The same namespace registers write methods and privileged collections; GET /wp/v2/users returned 401\n    rest_user_cannot_view anonymously. WordPress core authentication (cookie + X-WP-Nonce, or application\n    passwords) governs those, but Strata Oncology documents none of it publicly.\n  cors_allowed_headers:\n  - Authorization\n  - X-WP-Nonce\n  - Content-Disposition\n  - Content-MD5\n  - Content-Type\n- surface: Strata Request Portal\n  url: https://portal.strataoncology.com/\n  authentication: credentialed web login (account requested via https://strataoncology.com/create-account/)\n  machine_readable_contract: none\n  evidence: >-\n    Single-page app on S3/CloudFront; /.well-known/openid-configuration, /.well-known/oauth-authorization-server\n    and /.well-known/oauth-protected-resource all returned 403 (S3 AccessDenied), i.e. no OIDC or OAuth\n    discovery document is published.\n- surface: Strata Assistant (Epic App Orchard)\n  authentication:\
  \ governed by Epic's app distribution model\n  machine_readable_contract: none\n  evidence: >-\n    Announced 2021-05-18 as an app integrated within Epic to pre-populate StrataNGS requisitions from EMR data.\n    Strata Oncology's announcement names no integration standard (no SMART on FHIR / HL7 FHIR claim), and no\n    public contract is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strata-oncology/refs/heads/main/authentication/strata-oncology-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Precision Medicine
- Oncology
- Genomics
- Diagnostics
- Laboratory
- Life Sciences
- Biomarkers
- Clinical Trials
---
