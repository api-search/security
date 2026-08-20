---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Builder Prime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Builder Prime secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Builder Prime
provider_slug: builder-prime
scheme_count: 1
schemes:
- description: A per-tenant secret key generated inside the Builder Prime application under Admin > Integrations > Open API. The key is displayed exactly once at generation time and cannot be retrieved again — a lost key must be regenerated. Each key is given a name (typically the name of the sending application) and a set of named permissions.
  in: header
  issuance:
    displayed_once: true
    path: Admin > Integrations > Open API > Generate New API Key
    requires_authenticated_tenant: true
    rotatable: true
    rotation_method: generate-a-new-key
    self_service: true
  name: OpenApiSecretKey
  parameter_name: x-api-key
  sources:
  - https://www.builderprime.com/blog/open-api-documentation
  type: apiKey
  x-evidence:
  - basis: Named in the (now removed) Builder Prime knowledge-base articles "Working with Clients through the API" and "Working with Employees through the API", and independently used by the third-party n8n community node n8n-nodes-builderprime, whose published source sends the tenant key in the x-api-key header against https://{subdomain}.builderprime.com.
    confidence: medium
    live_source_status:
      checked: '2026-08-08'
      http_status: 404
      url: https://help.builderprime.com/bp-knowledgebase/working-with-clients-through-the-api-1-0
    what: header name x-api-key
  - basis: 'Unauthenticated GET of the live resource paths returns HTTP 401 with the body {"success":false,"errors":[{"code":"API_GENERAL","message":"Unauthorized: Invalid key"}]}, while an unknown path on the same host returns a structurally different 404 envelope. The 401 is therefore real authentication, not a catch-all.'
    confidence: high
    live_source_status:
      checked: '2026-08-08'
      http_status: 401
      url: https://developer.builderprime.com/api/employees/v1
    what: an API key is required on every resource
slug: builder-prime-authentication
source_filename: builder-prime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: searched\nsource: https://www.builderprime.com/blog/open-api-documentation\ndocs: https://www.builderprime.com/blog/open-api-documentation\nnote: >-\n  Derived from the provider's own live \"Open API Documentation\" page plus\n  unauthenticated probes of the live API host. Builder Prime publishes no OpenAPI\n  definition, so there are no machine-readable securitySchemes to derive from —\n  this profile is assembled from published prose and observed 401 responses.\n\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  multi_tenant: true\n\nschemes:\n- name: OpenApiSecretKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    A per-tenant secret key generated inside the Builder Prime application under\n    Admin > Integrations > Open API. The key is displayed exactly once at\n    generation time and cannot be retrieved again — a lost key must be\n    regenerated. Each key is given a name (typically\
  \ the name of the sending\n    application) and a set of named permissions.\n  issuance:\n    self_service: true\n    requires_authenticated_tenant: true\n    path: Admin > Integrations > Open API > Generate New API Key\n    displayed_once: true\n    rotatable: true\n    rotation_method: generate-a-new-key\n  sources:\n  - https://www.builderprime.com/blog/open-api-documentation\n  x-evidence:\n  - what: header name x-api-key\n    confidence: medium\n    basis: >-\n      Named in the (now removed) Builder Prime knowledge-base articles\n      \"Working with Clients through the API\" and \"Working with Employees through\n      the API\", and independently used by the third-party n8n community node\n      n8n-nodes-builderprime, whose published source sends the tenant key in the\n      x-api-key header against https://{subdomain}.builderprime.com.\n    live_source_status:\n      url: https://help.builderprime.com/bp-knowledgebase/working-with-clients-through-the-api-1-0\n      http_status:\
  \ 404\n      checked: '2026-08-08'\n  - what: an API key is required on every resource\n    confidence: high\n    basis: >-\n      Unauthenticated GET of the live resource paths returns HTTP 401 with the\n      body {\"success\":false,\"errors\":[{\"code\":\"API_GENERAL\",\"message\":\"Unauthorized:\n      Invalid key\"}]}, while an unknown path on the same host returns a\n      structurally different 404 envelope. The 401 is therefore real\n      authentication, not a catch-all.\n    live_source_status:\n      url: https://developer.builderprime.com/api/employees/v1\n      http_status: 401\n      checked: '2026-08-08'\n\ntenancy:\n  model: subdomain-per-customer\n  description: >-\n    The API host is the customer's own Builder Prime subdomain — the first label\n    of the URL used to sign in to the web app. Builder Prime instructs customers\n    to send that subdomain to the integrating application alongside the secret\n    key, so the tenant is carried by the host rather than by a header\
  \ or a path\n    segment.\n  documented_pattern: https://{subdomain}.builderprime.com\n  example_given_by_provider: https://johnsfloors.builderprime.com\n\npermissions:\n  model: named-permissions-per-key\n  description: >-\n    Keys are scoped by selecting named permissions when the key is generated.\n    Builder Prime does not publish the full permission list on any public page;\n    the values below are the ones named in public material.\n  observed:\n  - name: clients.create\n    description: Create new clients / leads.\n    source: https://www.builderprime.com/blog/open-api-documentation\n    confidence: high\n  - name: employees.read\n    description: Read a single employee and list employees.\n    source: >-\n      Named in the removed knowledge-base article \"Working with Employees\n      through the API\" (live URL now returns 404).\n    confidence: medium\n  complete: false\n  gap: >-\n    Builder Prime publishes no public permissions/scopes reference. The complete\n    list\
  \ of key permissions is visible only inside an authenticated tenant on the\n    Admin > Integrations > Open API screen.\n\noauth2: false\nopenid_connect: false\nmutual_tls: false\nwell_known_discovery: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builder-prime/refs/heads/main/authentication/builder-prime-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- CRM
- Home Improvement
- Construction
- Contractors
- Remodeling
- Sales
- Estimating
- Project Management
- Lead Management
- Field Service
- Software-as-a-Service
---
