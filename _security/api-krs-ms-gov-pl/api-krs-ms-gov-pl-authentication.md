---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Krajowy Rejestr Sądowy (National Court Register), Poland Authentication
name_suffix: Authentication
oauth_flows: []
overview: Krajowy Rejestr Sądowy (National Court Register), Poland declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Krajowy Rejestr Sądowy (National Court Register), Poland
provider_slug: api-krs-ms-gov-pl
scheme_count: 1
schemes:
- description: 'No authentication: documented plain GET URLs, confirmed by an unauthenticated 200.'
  name: anonymous
  type: none
slug: api-krs-ms-gov-pl-authentication
source_filename: api-krs-ms-gov-pl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Open KRS API authentication\ngenerated: '2026-11-11'\nmethod: probed\nsource: https://prs.ms.gov.pl/krs/openApi\ndocs: https://prs.ms.gov.pl/krs/openApi\nschemes:\n- type: none\n  name: anonymous\n  description: 'No authentication: documented plain GET URLs, confirmed by an unauthenticated\n    200.'\nanonymous: true\nnote: The docs list each service as a plain GET URL with no key, token or registration\n  step; an unauthenticated GET of https://api-krs.ms.gov.pl/api/krs/OdpisAktualny/0000019193?rodzaj=aktualny&format=json\n  returned 200 application/json (51,412 bytes) on 2026-11-11.\n"
source_yaml_url: https://artifacts.apis.io/api-krs-ms-gov-pl/authentication/api-krs-ms-gov-pl-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Government
- Business Registry
- Open Data
- Poland
- Legal Entities
- Europe
---
