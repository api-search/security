---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Nexus Mutual Cover Router API
  slug: nexus-mutual-cover-router-api
  spec_type: OpenAPI
  url: https://api.nexusmutual.io/v2/api/docs/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nexusmutual.io
  spf: true
hosts:
- cert_expires: Sep 14 15:05:57 2026 GMT
  host: docs.nexusmutual.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:57:18 2026 GMT
  host: api.nexusmutual.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Nexus Mutual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexus Mutual, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nexus Mutual
provider_slug: nexus-mutual
slug: nexus-mutual-domain-security
source_filename: nexus-mutual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.nexusmutual.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:05:57 2026 GMT\n  hsts: false\n- host: api.nexusmutual.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:57:18 2026 GMT\n  hsts: null\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: nexusmutual.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexus-mutual/refs/heads/main/security/nexus-mutual-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Decentralized Insurance
- DeFi
- Ethereum
- Smart Contract Cover
- Crypto Insurance
- Protocol Protection
- Staking
- Claims
---
