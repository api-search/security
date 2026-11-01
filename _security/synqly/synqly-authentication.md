---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synqly-openapi-generated.yml
  format: yaml
  label: Synqly API
  slug: synqly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synqly/openapi/_ae-authored/synqly-openapi-generated.yml
auth_types: []
description: Authentication methods for Synqly providers as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Synqly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synqly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Synqly
provider_slug: synqly
scheme_count: 2
schemes:
- evidence: The CrowdStrike Cloud Security Provider uses OAuth 2.0 client credentials for authentication, and requires the use of a Client ID and Secret.
  flows:
  - client_credentials
  how_to_obtain: Create an API Client in the CrowdStrike Falcon Console and generate a Client ID and Secret.
  name: CrowdStrike Cloud Security OAuth2 Client Credentials
  scopes:
  - CSPM registration
  - Cloud Security Assets
  type: oauth2
- evidence: ClientId and ClientSecret are required in order to make requests using the OAuth2.0 workflow to CrowdStrike's API client.
  flows:
  - client_credentials
  how_to_obtain: Create an API Client in the CrowdStrike Falcon Console, select required scopes, and store the generated Client ID and Secret.
  name: CrowdStrike EDR OAuth2 Client Credentials
  scopes:
  - Alerts
  - Hosts
  - Assets
  - IOC Management
  - Custom IOA Rules
  - Zero Trust Assessment
  - Real Time Response
  - Real Time Response (Admin)
  type: oauth2
slug: synqly-authentication
source_filename: synqly-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.synqly.com/guides/provider-configuration/axonius-asset-setup.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.synqly.com/guides/provider-configuration/axonius-asset-setup.md\nsources:\n- https://docs.synqly.com/guides/provider-configuration/axonius-asset-setup.md\n- https://docs.synqly.com/guides/provider-configuration/azure-monitor-logs.md\n- https://docs.synqly.com/guides/provider-configuration/crowdstrike-cloudsecurity-setup.md\n- https://docs.synqly.com/guides/provider-configuration/crowdstrike-edr-setup.md\ndescription: Authentication methods for Synqly providers as documented.\nschemes:\n- type: oauth2\n  name: CrowdStrike Cloud Security OAuth2 Client Credentials\n  evidence: The CrowdStrike Cloud Security Provider uses OAuth 2.0 client credentials for authentication, and requires the use of a Client ID\n    and Secret.\n  flows:\n  - client_credentials\n  scopes:\n  - CSPM registration\n  - Cloud Security Assets\n  how_to_obtain: Create an API Client in the CrowdStrike\
  \ Falcon Console and generate a Client ID and Secret.\n- type: oauth2\n  name: CrowdStrike EDR OAuth2 Client Credentials\n  evidence: ClientId and ClientSecret are required in order to make requests using the OAuth2.0 workflow to CrowdStrike's API client.\n  flows:\n  - client_credentials\n  scopes:\n  - Alerts\n  - Hosts\n  - Assets\n  - IOC Management\n  - Custom IOA Rules\n  - Zero Trust Assessment\n  - Real Time Response\n  - Real Time Response (Admin)\n  how_to_obtain: Create an API Client in the CrowdStrike Falcon Console, select required scopes, and store the generated Client ID and Secret.\ndocs: https://docs.synqly.com/guides/provider-configuration/axonius-asset-setup.md\n"
source_yaml_url: https://artifacts.apis.io/synqly/authentication/synqly-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Integration
- Automation
---
