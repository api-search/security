---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apinity.io
  spf: true
hosts:
- cert_expires: Aug 21 05:03:57 2026 GMT
  host: apinity.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 05:03:57 2026 GMT
  host: api.apinity.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apinity Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apinity.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apinity.io
provider_slug: apinity-io
slug: apinity-io-domain-security
source_filename: apinity-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apinity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:03:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apinity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:03:57 2026 GMT\n  hsts: null\ndomains:\n- domain: apinity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apinity-io/refs/heads/main/security/apinity-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Governance
- API Marketplace
- Compliance
- Discovery
- Integration Platform
---
