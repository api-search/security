---
api_specs:
- filename: audius-openapi.yml
  format: yaml
  label: Audius REST API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/openapi/audius-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: audius.co
  spf: true
- caa: []
  dmarc: true
  dnssec: true
  domain: audius.org
  spf: true
hosts:
- cert_expires: Oct  3 17:13:14 2026 GMT
  host: audius.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 07:52:07 2026 GMT
  host: docs.audius.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 20:48:33 2026 GMT
  host: api.audius.co
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Audius
provider_slug: audius
slug: audius-domain-security
source_filename: audius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audius.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:13:14 2026 GMT\n  hsts: false\n- host: docs.audius.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:52:07 2026 GMT\n  hsts: false\n- host: api.audius.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:48:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: audius.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n- domain: audius.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audius/refs/heads/main/security/audius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Music
- Streaming
- Decentralized
- Web3
- Open Source
- Blockchain
---
