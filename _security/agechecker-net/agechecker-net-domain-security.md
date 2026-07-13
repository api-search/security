---
api_specs:
- filename: agechecker-net-age-verification-openapi.yml
  format: yaml
  label: AgeChecker.Net Age Verification API
  slug: agechecker-net-age-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/openapi/agechecker-net-age-verification-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agechecker.net
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: agechecker.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.agechecker.net
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agechecker Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgeChecker.Net, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgeChecker.Net
provider_slug: agechecker-net
slug: agechecker-net-domain-security
source_filename: agechecker-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agechecker.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agechecker.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: agechecker.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/security/agechecker-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
---
