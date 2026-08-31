---
api_key_in:
- header
api_specs:
- filename: microsoft-net-packagecontent-api-openapi.yml
  format: yaml
  label: Microsoft .NET PackageContent API
  slug: microsoft-net-packagecontent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/openapi/microsoft-net-packagecontent-api-openapi.yml
- filename: microsoft-net-registration-api-openapi.yml
  format: yaml
  label: Microsoft .NET Registration API
  slug: microsoft-net-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/openapi/microsoft-net-registration-api-openapi.yml
- filename: microsoft-net-search-api-openapi.yml
  format: yaml
  label: Microsoft .NET Search API
  slug: microsoft-net-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/openapi/microsoft-net-search-api-openapi.yml
- filename: microsoft-net-serviceindex-api-openapi.yml
  format: yaml
  label: Microsoft .NET ServiceIndex API
  slug: microsoft-net-serviceindex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/openapi/microsoft-net-serviceindex-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Microsoft Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft .NET secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft .NET
provider_slug: microsoft-net
scheme_count: 1
schemes:
- applies_to:
  - PUT https://www.nuget.org/api/v2/package (push)
  - DELETE https://www.nuget.org/api/v2/package/{ID}/{VERSION} (unlist)
  - POST https://www.nuget.org/api/v2/package/{ID}/{VERSION} (relist)
  - PUT https://www.nuget.org/api/v2/symbolpackage (symbol push)
  description: NuGet API key (required only for PackagePublish push/delete operations).
  format: 'Recorded verbatim from the docs: "The API key is an opaque string gotten from the package source by the user and configured into the client. No particular string format is mandated but the length of the API key should not exceed a reasonable size for HTTP header values."'
  in: header
  issued_at: https://www.nuget.org/account/apikeys
  name: apiKey
  parameter: X-NuGet-ApiKey
  scoping: nuget.org lets an owner scope a key by glob pattern over package IDs and by action (push new, push new version, unlist), and set an expiry — a per-key permission model configured in the gallery UI rather than an OAuth scope surface exposed on the wire.
  sources:
  - openapi/microsoft-net-serviceindex-api-openapi.yml
  - openapi/microsoft-net-search-api-openapi.yml
  - openapi/microsoft-net-registration-api-openapi.yml
  - openapi/microsoft-net-packagecontent-api-openapi.yml
  test_vs_live: A NuGet API key carries no visible test/live marker, and the pre-production gallery at int.nugettest.org issues its own separate keys. The --source argument, not the key, is what separates a test push from a real one. See sandbox/.
  type: apiKey
slug: microsoft-net-authentication
source_filename: microsoft-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/microsoft-net-*-openapi.yml\ndocs: https://learn.microsoft.com/en-us/nuget/api/package-publish-resource\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  anonymous_read: true\nnote: >-\n  The defining fact about authentication on this API is how little of it there is. Every read operation\n  in openapi/ — service index, search, registration, flat container — is fully anonymous and sends no\n  credential at all; each spec carries `security: []`. The API key is required only on the write surface\n  (push, unlist/delete, relist, symbol push), which is documented in Microsoft's API reference but is not\n  modelled in openapi/. There is no OAuth, no OIDC, no scopes and no /.well-known/openid-configuration on\n  any provider host (all probed 404 or 400 on 2026-08-29; see well-known/), so scopes/ is intentionally\n  absent rather than empty.\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n  \
  \  parameter: X-NuGet-ApiKey\n    description: NuGet API key (required only for PackagePublish push/delete operations).\n    sources:\n      - openapi/microsoft-net-serviceindex-api-openapi.yml\n      - openapi/microsoft-net-search-api-openapi.yml\n      - openapi/microsoft-net-registration-api-openapi.yml\n      - openapi/microsoft-net-packagecontent-api-openapi.yml\n    format: >-\n      Recorded verbatim from the docs: \"The API key is an opaque string gotten from the package source by\n      the user and configured into the client. No particular string format is mandated but the length of\n      the API key should not exceed a reasonable size for HTTP header values.\"\n    issued_at: https://www.nuget.org/account/apikeys\n    scoping: >-\n      nuget.org lets an owner scope a key by glob pattern over package IDs and by action (push new,\n      push new version, unlist), and set an expiry — a per-key permission model configured in the\n      gallery UI rather than an OAuth scope surface\
  \ exposed on the wire.\n    applies_to:\n      - 'PUT https://www.nuget.org/api/v2/package (push)'\n      - 'DELETE https://www.nuget.org/api/v2/package/{ID}/{VERSION} (unlist)'\n      - 'POST https://www.nuget.org/api/v2/package/{ID}/{VERSION} (relist)'\n      - 'PUT https://www.nuget.org/api/v2/symbolpackage (symbol push)'\n    test_vs_live: >-\n      A NuGet API key carries no visible test/live marker, and the pre-production gallery at\n      int.nugettest.org issues its own separate keys. The --source argument, not the key, is what\n      separates a test push from a real one. See sandbox/.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_artifact: null\nscopes_note: No OAuth2 scheme exists on this API, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-net/refs/heads/main/authentication/microsoft-net-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- .NET
- C#
- Cloud
- Cross-Platform
- Developer Tools
- Microsoft
- Open-Source
---
