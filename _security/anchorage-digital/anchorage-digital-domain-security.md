---
api_specs:
- filename: anchorage-digital-openapi-original.json
  format: json
  label: Anchorage Digital API
  slug: anchorage-digital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage-digital/refs/heads/main/openapi/anchorage-digital-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anchorage.com
  spf: true
hosts:
- cert_expires: Sep 30 10:04:18 2026 GMT
  host: anchorage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anchorage Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchorage Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anchorage Digital
provider_slug: anchorage-digital
slug: anchorage-digital-domain-security
source_filename: anchorage-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:04:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anchorage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorage-digital/refs/heads/main/security/anchorage-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Custody
- Digital Assets
- Banking
- Trading
- Staking
- Settlement
- Institutional
- Blockchain
- Stablecoins
---
