---
api_specs:
- filename: georgia-institute-of-technology-sums.yaml
  format: yaml
  label: SUMS REST API
  slug: sums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/georgia-institute-of-technology/refs/heads/main/openapi/georgia-institute-of-technology-sums.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gatech.edu
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.gatech.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:20:15 2026 GMT
  host: repository.gatech.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:44:27 2026 GMT
  host: rnoc.gatech.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Georgia Institute Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Georgia Institute of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Georgia Institute of Technology
provider_slug: georgia-institute-of-technology
slug: georgia-institute-of-technology-domain-security
source_filename: georgia-institute-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gatech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: repository.gatech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:20:15 2026 GMT\n  hsts: false\n- host: rnoc.gatech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:44:27 2026 GMT\n  hsts: false\ndomains:\n- domain: gatech.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/georgia-institute-of-technology/refs/heads/main/security/georgia-institute-of-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- United States
---
