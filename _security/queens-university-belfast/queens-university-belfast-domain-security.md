---
api_specs:
- filename: queens-university-belfast-pure-api.yaml
  format: yaml
  label: Queen's University Belfast Research Portal (Pure REST API)
  slug: pure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/queens-university-belfast/refs/heads/main/openapi/queens-university-belfast-pure-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qub.ac.uk
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.qub.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 05:46:04 2026 GMT
  host: pure.qub.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:27:50 2026 GMT
  host: pureadmin.qub.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Queens University Belfast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Queen''s University Belfast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Queen's University Belfast
provider_slug: queens-university-belfast
slug: queens-university-belfast-domain-security
source_filename: queens-university-belfast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qub.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: pure.qub.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: pureadmin.qub.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:27:50 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: qub.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queens-university-belfast/refs/heads/main/security/queens-university-belfast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- OAI-PMH
- United Kingdom
- Northern Ireland
---
