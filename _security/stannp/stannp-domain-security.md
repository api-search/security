---
api_specs:
- filename: direct-mail-api
  format: yaml
  label: Stannp Direct Mail API
  slug: direct-mail-api
  spec_type: OpenAPI
  url: https://www.stannp.com/us/direct-mail-api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stannp.com
  spf: true
hosts:
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: www.stannp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 16:57:32 2026 GMT
  host: api-eu1.stannp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 16:57:32 2026 GMT
  host: api-us1.stannp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stannp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stannp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stannp
provider_slug: stannp
slug: stannp-domain-security
source_filename: stannp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stannp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-eu1.stannp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 16:57:32 2026 GMT\n  hsts: null\n- host: api-us1.stannp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 16:57:32 2026 GMT\n  hsts: null\ndomains:\n- domain: stannp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/security/stannp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Direct Mail
- Postcards
- Letters
- Print
- Physical Mail
- Marketing Automation
- Campaigns
---
