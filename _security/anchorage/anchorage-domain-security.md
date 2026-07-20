---
api_specs:
- filename: anchorage-v2-openapi-original.yml
  format: yaml
  label: Anchorage Digital REST API v2.0
  slug: anchorage-digital-rest-api-v20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/openapi/anchorage-v2-openapi-original.yml
- filename: anchorage-v3-openapi-original.yml
  format: yaml
  label: Anchorage Digital REST API v3
  slug: anchorage-digital-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/openapi/anchorage-v3-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: anchorage.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: anchorage-staging.com
  spf: false
hosts:
- cert_expires: Sep 30 10:04:18 2026 GMT
  host: anchorage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:16:13 2026 GMT
  host: api.anchorage-staging.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anchorage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchorage Digital, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Anchorage Digital
provider_slug: anchorage
slug: anchorage-domain-security
source_filename: anchorage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchorage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:04:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anchorage-staging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:16:13 2026 GMT\n  hsts: null\ndomains:\n- domain: anchorage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: anchorage-staging.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorage/refs/heads/main/security/anchorage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Digital Assets
- Custody
- Trading
- Staking
- Settlement
- Stablecoins
- Banking
- Institutional
---
