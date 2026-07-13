---
api_specs:
- filename: onomondo-openapi.yml
  format: yaml
  label: Onomondo SIMs API
  slug: onomondo-sims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-openapi.yml
- filename: onomondo-openapi.yml
  format: yaml
  label: Onomondo Usage & Traffic API
  slug: onomondo-usage-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-openapi.yml
- filename: onomondo-openapi.yml
  format: yaml
  label: Onomondo Networks API
  slug: onomondo-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-openapi.yml
- filename: onomondo-openapi.yml
  format: yaml
  label: Onomondo Webhooks & Notifications API
  slug: onomondo-webhooks-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-openapi.yml
- filename: onomondo-openapi.yml
  format: yaml
  label: Onomondo Apps & Connectors API
  slug: onomondo-apps-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onomondo.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: onomondo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 17:33:25 2026 GMT
  host: docs.onomondo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.onomondo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onomondo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onomondo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Onomondo
provider_slug: onomondo
slug: onomondo-domain-security
source_filename: onomondo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onomondo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.onomondo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 17:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.onomondo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: onomondo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/security/onomondo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Connectivity
- Cellular
- SIM
- Telecom
---
