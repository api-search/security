---
api_specs:
- filename: osmaura-prospect-openapi.yml
  format: yaml
  label: Osmaura Prospect API
  slug: osmaura-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/openapi/osmaura-prospect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osmaura.com
  spf: true
hosts:
- cert_expires: Oct 20 03:35:45 2026 GMT
  host: osmaura.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 22:10:04 2026 GMT
  host: dashboard.osmaura.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osmaura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osmaura, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Osmaura
provider_slug: osmaura
slug: osmaura-domain-security
source_filename: osmaura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osmaura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:35:45 2026 GMT\n  hsts: false\n- host: dashboard.osmaura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 22:10:04 2026 GMT\n  hsts: false\ndomains:\n- domain: osmaura.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/security/osmaura-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- Legal Tech
- Artificial Intelligence
- Sales Enablement
- Business Development
- Y Combinator
- Market Intelligence
- Data
- Government Data
- Prospecting
---
