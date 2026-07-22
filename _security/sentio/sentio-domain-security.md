---
api_specs:
- filename: sentio-openapi.yml
  format: yaml
  label: Sentio API
  slug: sentio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentio.xyz
  spf: true
hosts:
- cert_expires: Oct 18 10:15:47 2026 GMT
  host: api.sentio.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sentio
provider_slug: sentio
slug: sentio-domain-security
source_filename: sentio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sentio.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 10:15:47 2026 GMT\n  hsts: null\ndomains:\n- domain: sentio.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/security/sentio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web3
- Blockchain
- Observability
- Analytics
- Data
- Indexing
- Monitoring
- Developer Tools
- Crypto
- API
---
