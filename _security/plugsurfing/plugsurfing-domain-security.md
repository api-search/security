---
api_specs:
- filename: plugsurfing-charging-key-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Key Orders API
  slug: plugsurfing-charging-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-charging-key-orders-api-openapi.yml
- filename: plugsurfing-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing Charging Keys API
  slug: plugsurfing-charging-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-charging-keys-api-openapi.yml
- filename: plugsurfing-drive-api-api-openapi.yml
  format: yaml
  label: Plugsurfing Drive API
  slug: plugsurfing-drive-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-drive-api-api-openapi.yml
- filename: plugsurfing-emp-charging-keys-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Charging Keys API
  slug: plugsurfing-emp-charging-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-charging-keys-api-openapi.yml
- filename: plugsurfing-emp-fleets-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Fleets API
  slug: plugsurfing-emp-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-fleets-api-openapi.yml
- filename: plugsurfing-emp-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Geosearch API
  slug: plugsurfing-emp-geosearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-geosearch-api-openapi.yml
- filename: plugsurfing-emp-orders-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Orders API
  slug: plugsurfing-emp-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-orders-api-openapi.yml
- filename: plugsurfing-emp-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing EMP Sessions API
  slug: plugsurfing-emp-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-emp-sessions-api-openapi.yml
- filename: plugsurfing-geosearch-api-openapi.yml
  format: yaml
  label: Plugsurfing Geosearch API
  slug: plugsurfing-geosearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-geosearch-api-openapi.yml
- filename: plugsurfing-payment-options-api-openapi.yml
  format: yaml
  label: Plugsurfing Payment Options API
  slug: plugsurfing-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-payment-options-api-openapi.yml
- filename: plugsurfing-remote-charging-api-openapi.yml
  format: yaml
  label: Plugsurfing Remote Charging API
  slug: plugsurfing-remote-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-remote-charging-api-openapi.yml
- filename: plugsurfing-sessions-api-openapi.yml
  format: yaml
  label: Plugsurfing Sessions API
  slug: plugsurfing-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-sessions-api-openapi.yml
- filename: plugsurfing-user-groups-api-openapi.yml
  format: yaml
  label: Plugsurfing User Groups API
  slug: plugsurfing-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-user-groups-api-openapi.yml
- filename: plugsurfing-users-api-openapi.yml
  format: yaml
  label: Plugsurfing Users API
  slug: plugsurfing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-users-api-openapi.yml
- filename: plugsurfing-vouchers-api-openapi.yml
  format: yaml
  label: Plugsurfing Vouchers API
  slug: plugsurfing-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/plugsurfing-vouchers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plugsurfing.com
  spf: true
hosts:
- cert_expires: Nov 30 12:31:21 2026 GMT
  host: www.plugsurfing.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plugsurfing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plugsurfing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plugsurfing
provider_slug: plugsurfing
slug: plugsurfing-domain-security
source_filename: plugsurfing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plugsurfing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 12:31:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: plugsurfing.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/security/plugsurfing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EVCharging
- Roaming
- Europe
---
