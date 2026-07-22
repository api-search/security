---
api_specs:
- filename: re-openapi.yml
  format: yaml
  label: Re Protocol API
  slug: re-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/re/refs/heads/main/openapi/re-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: re.xyz
  spf: true
hosts:
- cert_expires: Aug 24 01:38:43 2026 GMT
  host: re.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 00:33:26 2026 GMT
  host: docs.re.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 18:23:01 2026 GMT
  host: api.re.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Re Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Re, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Re
provider_slug: re
slug: re-domain-security
source_filename: re-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: re.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:38:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.re.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.re.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:23:01 2026 GMT\n  hsts: null\ndomains:\n- domain: re.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re/refs/heads/main/security/re-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Reinsurance
- Insurance
- DeFi
- Blockchain
- Real World Assets
- Stablecoin
- Yield
- Onchain
---
