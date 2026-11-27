---
api_specs:
- filename: derod-org-json-rpc-api-openapi.yml
  format: yaml
  label: DERO Project Json Rpc API
  slug: derod-org-json-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/derod-org/openapi/derod-org-json-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: derod.org
  spf: true
hosts:
- cert_expires: Jan 30 03:38:10 2027 GMT
  host: derod.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DERO Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DERO Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DERO Project
provider_slug: derod-org
slug: derod-org-domain-security
source_filename: derod-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: derod.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 03:38:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: derod.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/derod-org/security/derod-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Privacy
- Smart Contracts
- Homomorphic Encryption
- decentralized-apps
---
