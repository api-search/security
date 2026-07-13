---
api_specs:
- filename: moesif-openapi.yml
  format: yaml
  label: Moesif Management API
  slug: moesif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moesif.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: moesif.net
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.moesif.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.moesif.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.moesif.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moesif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moesif, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moesif
provider_slug: moesif
slug: moesif-domain-security
source_filename: moesif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moesif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moesif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.moesif.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: moesif.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moesif.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/security/moesif-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Monitoring
- Monetization
- Governance
- Observability
- Billing
- AI Agents
- LLM Analytics
- OpenTelemetry
- Developer Portal
- Platform
- Insights
---
