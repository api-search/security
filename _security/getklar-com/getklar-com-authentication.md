---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getklar-com-openapi-generated.yml
  format: yaml
  label: Klar API
  slug: getklar-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getklar-com/openapi/_ae-authored/getklar-com-openapi-generated.yml
auth_types: []
description: 'Klar uses Bearer authentication. Pass your token in the `Authorization` header of every request:'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Klar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klar declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Klar
provider_slug: getklar-com
scheme_count: 1
schemes:
- evidence: 'Klar uses Bearer authentication. Pass your token in the `Authorization` header of every request:'
  header: Authorization
  how_to_obtain: Connect a Klar API or Klar Returns data source in Settings → Store Configurator → Data Sources, then copy the Access Token from the data source’s Access Token tab.
  location: header
  name: Bearer
  type: http-bearer
slug: getklar-com-authentication
source_filename: getklar-com-authentication.yml
source_heading: Authentication Profile
source_url: https://help.getklar.com/en/articles/9345493-api-authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.getklar.com/en/articles/9345493-api-authentication.md\nsources:\n- https://help.getklar.com/en/articles/9345493-api-authentication.md\n- https://help.getklar.com/de/articles/10412008-a-b-testing-setup-report.md\ndescription: 'Klar uses Bearer authentication. Pass your token in the `Authorization` header of every request:'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Klar uses Bearer authentication. Pass your token in the `Authorization` header of every request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Connect a Klar API or Klar Returns data source in Settings → Store Configurator → Data Sources, then copy the Access Token from\n    the data source’s Access Token tab.\nnote: The token is a JWT as shown on the page.\ndocs: https://help.getklar.com/en/articles/9345493-api-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/getklar-com/authentication/getklar-com-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Marketing
- Analytics
- Attribution
- Software-as-a-Service
---
