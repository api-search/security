---
api_specs:
- filename: bloqit-bloqs-api-openapi.yml
  format: yaml
  label: Bloqit Bloqs API
  slug: bloqit-bloqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloqit/refs/heads/main/openapi/bloqit-bloqs-api-openapi.yml
- filename: bloqit-public-api-openapi.yml
  format: yaml
  label: Bloqit Public API
  slug: bloqit-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloqit/refs/heads/main/openapi/bloqit-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bloq.it
  spf: true
hosts:
- cert_expires: Nov  9 01:29:26 2026 GMT
  host: www.bloq.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bloqit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloqit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bloqit
provider_slug: bloqit
slug: bloqit-domain-security
source_filename: bloqit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloq.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:29:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bloq.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloqit/refs/heads/main/security/bloqit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Data Storage
- API Platform
- Fintech
- Lisbon
---
