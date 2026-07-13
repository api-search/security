---
api_specs:
- filename: candid-essentials-api-openapi.yml
  format: yaml
  label: Candid Essentials API
  slug: essentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candid/refs/heads/main/openapi/candid-essentials-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: candid.org
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: candid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 08:30:01 2026 GMT
  host: developer.candid.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.candid.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Candid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Candid
provider_slug: candid
slug: candid-domain-security
source_filename: candid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: candid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: developer.candid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:30:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.candid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: candid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candid/refs/heads/main/security/candid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Charities
- Donations
- Non-Profits
- Philanthropy
- Foundations
- Grants
- 990s
- Demographics
---
