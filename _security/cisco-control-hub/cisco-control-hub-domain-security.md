---
api_specs:
- filename: cisco-control-hub-adminauditevents-api-openapi.yml
  format: yaml
  label: Cisco Control Hub AdminAuditEvents API
  slug: cisco-control-hub-adminauditevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-adminauditevents-api-openapi.yml
- filename: cisco-control-hub-devices-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Devices API
  slug: cisco-control-hub-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-devices-api-openapi.yml
- filename: cisco-control-hub-licenses-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Licenses API
  slug: cisco-control-hub-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-licenses-api-openapi.yml
- filename: cisco-control-hub-locations-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Locations API
  slug: cisco-control-hub-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-locations-api-openapi.yml
- filename: cisco-control-hub-organizations-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Organizations API
  slug: cisco-control-hub-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-organizations-api-openapi.yml
- filename: cisco-control-hub-people-api-openapi.yml
  format: yaml
  label: Cisco Control Hub People API
  slug: cisco-control-hub-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-people-api-openapi.yml
- filename: cisco-control-hub-workspaces-api-openapi.yml
  format: yaml
  label: Cisco Control Hub Workspaces API
  slug: cisco-control-hub-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/openapi/cisco-control-hub-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "identrust.com"
  - 128 iodef "mailto:infosec@cisco.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webex.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: webexapis.com
  spf: false
hosts:
- cert_expires: Dec 21 09:08:54 2026 GMT
  host: developer.webex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 08:51:15 2026 GMT
  host: webexapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cisco Control Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cisco Control Hub, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cisco Control Hub
provider_slug: cisco-control-hub
slug: cisco-control-hub-domain-security
source_filename: cisco-control-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.webex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webexapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:51:15 2026 GMT\n  hsts: null\ndomains:\n- domain: webex.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"identrust.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webexapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-control-hub/refs/heads/main/security/cisco-control-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Administration
- Calling
- Collaboration
- Communications
- Device Management
- Identity Management
- Licenses
- Reporting
- Webex
---
