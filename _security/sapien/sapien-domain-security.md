---
api_specs:
- filename: sapien-poq-openapi-original.json
  format: json
  label: Sapien Proof of Quality Developer API
  slug: sapien-proof-of-quality-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sapien/refs/heads/main/openapi/sapien-poq-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sapien.io
  spf: true
- caa:
  - 0 issuewild "certainly.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: railway.app
  spf: true
hosts:
- cert_expires: Sep  4 03:47:05 2026 GMT
  host: www.sapien.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 21:46:21 2026 GMT
  host: docs.sapien.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:01:29 2026 GMT
  host: sapien-poq.up.railway.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sapien Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapien, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sapien
provider_slug: sapien
slug: sapien-domain-security
source_filename: sapien-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sapien.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:47:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sapien.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:46:21 2026 GMT\n  hsts: false\n- host: sapien-poq.up.railway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:01:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sapien.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: railway.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapien/refs/heads/main/security/sapien-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Data Quality
- Data Labeling
- Machine Learning
- Human in the Loop
- Attestation
- Blockchain
- Consensus
- MCP
---
