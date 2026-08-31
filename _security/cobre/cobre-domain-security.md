---
api_specs:
- filename: cobre-events-asyncapi.yml
  format: yaml
  label: Cobre Platform API
  slug: cobre-platform-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cobre/refs/heads/main/asyncapi/cobre-events-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cobre.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cobre.co
  spf: true
hosts:
- cert_expires: Aug 31 21:03:47 2026 GMT
  host: www.cobre.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 00:03:50 2026 GMT
  host: docs.cobre.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 20 18:50:19 2026 GMT
  host: api.cobre.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cobre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobre, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cobre
provider_slug: cobre
slug: cobre-domain-security
source_filename: cobre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cobre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cobre.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 00:03:50 2026 GMT\n  hsts: false\n- host: api.cobre.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:50:19 2026 GMT\n  hsts: null\ndomains:\n- domain: cobre.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cobre.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobre/refs/heads/main/security/cobre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Treasury
- Money Movement
- Cross Border Payments
- FX
- Stablecoins
- Banking
- Latin America
- Colombia
- Mexico
---
