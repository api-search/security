---
api_specs:
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Printers
  slug: formlabs-web-api-printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Prints
  slug: formlabs-web-api-prints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Consumables
  slug: formlabs-web-api-consumables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Events
  slug: formlabs-web-api-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Groups
  slug: formlabs-web-api-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: formlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: formlabs.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: formlabs-dashboard-api-resources.s3.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 10:28:15 2026 GMT
  host: api.formlabs.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formlabs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Formlabs
provider_slug: formlabs
slug: formlabs-domain-security
source_filename: formlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: formlabs-dashboard-api-resources.s3.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: api.formlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: formlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/security/formlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- 3D Printing
- Additive Manufacturing
- SLA
- SLS
- Hardware
- Dashboard
---
