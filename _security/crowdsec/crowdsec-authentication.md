---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for CrowdSec APIs as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Crowdsec Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crowdsec declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Crowdsec
provider_slug: crowdsec
scheme_count: 2
schemes:
- evidence: you can use it to authenticate requests to the CrowdSec Service API by including it in the `x-api-key` header of your HTTP requests.
  header: x-api-key
  how_to_obtain: Create a CTI API key in the CrowdSec Console (see page 3) or generate a service API key via the Console UI.
  location: header
  name: API Key
  type: apiKey
- evidence: 'TLS client certificates: they are used to authenticate Remediation Components (bouncers) and Log Processors (machines).'
  how_to_obtain: Generate a client certificate for a bouncer or agent using `cscli bouncers add` or `cscli machines add`, then configure the certificate paths in the LAPI and agent configuration files.
  name: TLS client certificate
  type: mtls
slug: crowdsec-authentication
source_filename: crowdsec-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.crowdsec.net/docs/next/local_api/authentication.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.crowdsec.net/docs/next/local_api/authentication.md\nsources:\n- https://docs.crowdsec.net/docs/next/local_api/authentication.md\n- https://docs.crowdsec.net/docs/next/local_api/tls_auth.md\n- https://docs.crowdsec.net/u/console/ip_reputation/api_keys.md\n- https://docs.crowdsec.net/u/console/service_api/authentication.md\ndescription: Authentication methods for CrowdSec APIs as documented.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: you can use it to authenticate requests to the CrowdSec Service API by including it in the `x-api-key` header of your HTTP requests.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a CTI API key in the CrowdSec Console (see page 3) or generate a service API key via the Console UI.\n- type: mtls\n  name: TLS client certificate\n  evidence: 'TLS client certificates: they are used to authenticate Remediation Components\
  \ (bouncers) and Log Processors (machines).'\n  how_to_obtain: Generate a client certificate for a bouncer or agent using `cscli bouncers add` or `cscli machines add`, then configure the certificate\n    paths in the LAPI and agent configuration files.\ndocs: https://docs.crowdsec.net/docs/next/local_api/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdsec/refs/heads/main/authentication/crowdsec-authentication.yml
summary_line: 2 schemes
tags:
- Security
- Threat Intelligence
- Open Source
- Community
- Automation
- CrowdSec
---
