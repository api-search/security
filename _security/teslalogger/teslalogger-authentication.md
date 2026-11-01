---
anonymous_access: false
api_key_in: []
api_specs:
- filename: teslalogger-openapi-generated.yml
  format: yaml
  label: TeslaLogger (self-hosted) API
  slug: teslalogger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teslalogger/openapi/_ae-authored/teslalogger-openapi-generated.yml
auth_types: []
description: Authentication is performed via the new Tesla Fleet API. The user logs in with their Tesla account email, password, and MFA code, after which an Access Token is provided for the Fleet API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Teslalogger Authentication
name_suffix: Authentication
oauth_flows: []
overview: TeslaLogger (self-hosted) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TeslaLogger (self-hosted)
provider_slug: teslalogger
scheme_count: 1
schemes:
- evidence: Seit Februar 2024 wird empfohlen, die Anmeldung über das neue Tesla Fleet API durchzuführen.
  flows:
  - authorization_code
  how_to_obtain: Enter the Tesla account email, password, and MFA code in the admin panel; after successful login the Access Token fields are populated.
  name: Tesla Fleet API
  type: oauth2
slug: teslalogger-authentication
source_filename: teslalogger-authentication.yml
source_heading: Authentication Profile
source_url: https://teslalogger.de/docs/installation/initial-setup/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://teslalogger.de/docs/installation/initial-setup/\nsources:\n- https://teslalogger.de/docs/installation/initial-setup/\n- https://teslalogger.de/docs/installation/initial-setup-without-backup/\n- https://teslalogger.de/docs/installation/initial-setup-with-backup/\n- https://teslalogger.de/en/docs/installation/raspberry-install/\ndescription: Authentication is performed via the new Tesla Fleet API. The user logs in with their Tesla account email, password, and MFA code,\n  after which an Access Token is provided for the Fleet API.\nschemes:\n- type: oauth2\n  name: Tesla Fleet API\n  evidence: Seit Februar 2024 wird empfohlen, die Anmeldung über das neue Tesla Fleet API durchzuführen.\n  flows:\n  - authorization_code\n  how_to_obtain: Enter the Tesla account email, password, and MFA code in the admin panel; after successful login the Access Token fields are\n    populated.\n\
  docs: https://teslalogger.de/docs/installation/initial-setup/\n"
source_yaml_url: https://artifacts.apis.io/teslalogger/authentication/teslalogger-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automotive
- DataLogging
- OpenSource
- Tesla
---
