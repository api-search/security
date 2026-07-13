---
api_specs:
- filename: eindhoven-university-of-technology-pure-web-service.yaml
  format: yaml
  label: TU/e Pure Web Service (Research API)
  slug: pure-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eindhoven-university-of-technology/refs/heads/main/openapi/eindhoven-university-of-technology-pure-web-service.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tue.nl
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: www.tue.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:03:20 2026 GMT
  host: research.tue.nl
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 05:37:14 2026 GMT
  host: pure.tue.nl
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eindhoven University Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eindhoven University of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Eindhoven University of Technology
provider_slug: eindhoven-university-of-technology
slug: eindhoven-university-of-technology-domain-security
source_filename: eindhoven-university-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tue.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: research.tue.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:03:20 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: pure.tue.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:37:14 2026 GMT\n  hsts: null\ndomains:\n- domain: tue.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eindhoven-university-of-technology/refs/heads/main/security/eindhoven-university-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Netherlands
- Europe
---
