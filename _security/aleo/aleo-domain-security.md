---
api_specs:
- filename: aleo-node-api-openapi.yml
  format: yaml
  label: Aleo Node REST API
  slug: aleo-node-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/openapi/aleo-node-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aleo.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: provable.com
  spf: true
hosts:
- cert_expires: Sep 22 23:15:56 2026 GMT
  host: docs.aleo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:03:17 2026 GMT
  host: api.explorer.provable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aleo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aleo
provider_slug: aleo
slug: aleo-domain-security
source_filename: aleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aleo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:15:56 2026 GMT\n  hsts: false\n- host: api.explorer.provable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:03:17 2026 GMT\n  hsts: null\ndomains:\n- domain: aleo.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: provable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aleo/refs/heads/main/security/aleo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Zero-Knowledge
- Cryptography
- Privacy
- Web3
- Developer Tools
- Cryptocurrency
- Smart Contracts
---
