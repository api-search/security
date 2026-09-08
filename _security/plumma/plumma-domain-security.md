---
api_specs:
- filename: plumma-connect-openapi.yml
  format: yaml
  label: Plumma CONNECT API
  slug: plumma-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/openapi/plumma-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plumma.it
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.plumma.it
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: connect.plumma.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Plumma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plumma, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plumma
provider_slug: plumma
slug: plumma-domain-security
source_filename: plumma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plumma.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\n- host: connect.plumma.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: plumma.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plumma/refs/heads/main/security/plumma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecommunications
- Network APIs
- Italy
- Europe
- GSMA Open Gateway
- CAMARA
- API Aggregator
- Fraud Prevention
- Identity Verification
- SIM Swap
- KYC
- Age Verification
- Number Verification
- Telco Intelligence
- Software Development
---
