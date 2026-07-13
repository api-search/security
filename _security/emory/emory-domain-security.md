---
api_specs:
- filename: emory-digital-slide-archive.yaml
  format: yaml
  label: Emory Digital Slide Archive REST API
  slug: digital-slide-archive
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emory/refs/heads/main/openapi/emory-digital-slide-archive.yaml
description: ''
domains:
- caa:
  - 128 issuewild "amazon.com"
  - 128 issue "amazon.com"
  - 128 issuewild "sectigo.com"
  - 128 issue "sectigo.com"
  - 128 issue "ssl.com"
  - 128 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emory.edu
  spf: true
hosts:
- cert_expires: Aug  5 20:49:01 2026 GMT
  host: www.emory.edu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 06:10:37 2026 GMT
  host: computablebrain.emory.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:55:27 2026 GMT
  host: canvas.emory.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emory University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Emory University
provider_slug: emory
slug: emory-domain-security
source_filename: emory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emory.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 20:49:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: computablebrain.emory.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:10:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: canvas.emory.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:55:27 2026 GMT\n  hsts: null\ndomains:\n- domain: emory.edu\n  dnssec: false\n  caa:\n  - 128 issuewild \"amazon.com\"\n  - 128 issue \"amazon.com\"\n  - 128 issuewild \"sectigo.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"ssl.com\"\n  - 128 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emory/refs/heads/main/security/emory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Libraries
- United States
- Atlanta
---
