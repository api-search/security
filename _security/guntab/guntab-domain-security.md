---
api_specs:
- filename: guntab-openapi.yml
  format: yaml
  label: GunTab REST API
  slug: guntab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guntab/refs/heads/main/openapi/guntab-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: guntab.com
  spf: true
hosts:
- cert_expires: Aug 30 00:57:16 2026 GMT
  host: www.guntab.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:52:29 2026 GMT
  host: api.guntab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guntab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GunTab, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: GunTab
provider_slug: guntab
slug: guntab-domain-security
source_filename: guntab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guntab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:57:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.guntab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:52:29 2026 GMT\n  hsts: null\ndomains:\n- domain: guntab.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guntab/refs/heads/main/security/guntab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Firearms
- Marketplace
- Payments
---
