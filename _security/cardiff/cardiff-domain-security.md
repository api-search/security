---
api_specs:
- filename: cardiff-courses.yaml
  format: yaml
  label: Courses
  slug: courses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses.yaml
- filename: cardiff-modules.yaml
  format: yaml
  label: Modules
  slug: modules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules.yaml
- filename: cardiff-lookups.yaml
  format: yaml
  label: Lookups
  slug: lookups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-lookups.yaml
- filename: cardiff-publications.yaml
  format: yaml
  label: Publications
  slug: publications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications.yaml
- filename: cardiff-echo.yaml
  format: yaml
  label: EchoTest
  slug: echo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-echo.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cardiff.ac.uk
  spf: true
hosts:
- cert_expires: Sep  2 00:49:21 2026 GMT
  host: www.cardiff.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:14:17 2026 GMT
  host: data.cardiff.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.data.cardiff.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardiff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardiff University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cardiff University
provider_slug: cardiff
slug: cardiff-domain-security
source_filename: cardiff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:49:21 2026 GMT\n  hsts: null\n- host: data.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 02:14:17 2026 GMT\n  hsts: null\n- host: api.data.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cardiff.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/security/cardiff-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Wales
- Open Data
- Courses
- Research
---
