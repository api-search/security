---
api_specs:
- filename: university-of-manchester-pure-rest.yaml
  format: yaml
  label: Pure CRIS REST API
  slug: pure-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-pure-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: manchester.ac.uk
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.manchester.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 02:50:22 2026 GMT
  host: research.manchester.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:45:31 2026 GMT
  host: pure.manchester.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Manchester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Manchester, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Manchester
provider_slug: university-of-manchester
slug: university-of-manchester-domain-security
source_filename: university-of-manchester-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.manchester.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: research.manchester.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: pure.manchester.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: manchester.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/security/university-of-manchester-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United Kingdom
---
