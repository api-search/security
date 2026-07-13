---
api_specs:
- filename: cornell-codi-classes.yaml
  format: yaml
  label: Cornell Open Data Initiative (CODI)
  slug: codi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/openapi/cornell-codi-classes.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cornell.edu
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.cornell.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: classes.cornell.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:10:15 2026 GMT
  host: guides.library.cornell.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cornell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cornell University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cornell University
provider_slug: cornell
slug: cornell-domain-security
source_filename: cornell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cornell.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\n- host: classes.cornell.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: guides.library.cornell.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:10:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cornell.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cornell/refs/heads/main/security/cornell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Course Catalog
- Library
- Research
- United States
---
