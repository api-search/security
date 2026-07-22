---
api_specs:
- filename: quinyx-api-v3-openapi.yml
  format: yaml
  label: Quinyx API v3
  slug: quinyx-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v3-openapi.yml
- filename: quinyx-api-v2-openapi.yml
  format: yaml
  label: Quinyx API v2
  slug: quinyx-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-api-v2-openapi.yml
- filename: quinyx-userapi-v2-openapi.yml
  format: yaml
  label: Quinyx User API v2
  slug: quinyx-user-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/openapi/quinyx-userapi-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@quinyx.com"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quinyx.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.quinyx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api-rc.quinyx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: user-api.quinyx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quinyx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quinyx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quinyx
provider_slug: quinyx
slug: quinyx-domain-security
source_filename: quinyx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.quinyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: api-rc.quinyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: user-api.quinyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quinyx.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admin@quinyx.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quinyx/refs/heads/main/security/quinyx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Workforce Management
- Scheduling
- Human Resources
- Time Tracking
- Forecasting
- Employee Engagement
- Retail
- Hospitality
- Company
---
