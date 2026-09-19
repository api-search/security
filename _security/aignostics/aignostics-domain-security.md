---
api_specs:
- filename: aignostics-public-api-openapi.yml
  format: yaml
  label: Aignostics Public API
  slug: aignostics-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/openapi/aignostics-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aignostics.com
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Nov  9 04:02:54 2026 GMT
  host: www.aignostics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:31:53 2026 GMT
  host: aignostics.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 04:06:08 2026 GMT
  host: platform.aignostics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aignostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aignostics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aignostics
provider_slug: aignostics
slug: aignostics-domain-security
source_filename: aignostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aignostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:02:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aignostics.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.aignostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 04:06:08 2026 GMT\n  hsts: null\ndomains:\n- domain: aignostics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/security/aignostics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Health
- Healthcare
- Life Sciences
- Pathology
- Medical Imaging
- Digital Pathology
- Oncology
- Biotechnology
- Research
- Germany
---
