---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Synup API
  slug: synup-api
  spec_type: OpenAPI
  url: https://www.synup.dev/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synup.com
  spf: true
hosts:
- cert_expires: Sep 28 23:30:16 2026 GMT
  host: www.synup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: developer.synup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: app.synup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synup, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Synup
provider_slug: synup
slug: synup-domain-security
source_filename: synup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:30:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.synup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\n- host: app.synup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: synup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synup/refs/heads/main/security/synup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Local Marketing
- Listings Management
- Reputation Management
- Local SEO
- Reviews
- Social Media
- Analytics
---
