---
api_specs:
- filename: johns-hopkins-university-sis-course-search.yaml
  format: yaml
  label: Self-Service Public Course Search API (SIS)
  slug: sis-course-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-sis-course-search.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jhu.edu
  spf: true
hosts:
- cert_expires: Oct  7 21:28:07 2026 GMT
  host: www.jhu.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:27:36 2026 GMT
  host: api.hub.jhu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:52:09 2026 GMT
  host: sis.jhu.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Johns Hopkins University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Johns Hopkins University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Johns Hopkins University
provider_slug: johns-hopkins-university
slug: johns-hopkins-university-domain-security
source_filename: johns-hopkins-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jhu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:28:07 2026 GMT\n  hsts: null\n- host: api.hub.jhu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:27:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sis.jhu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:52:09 2026 GMT\n  hsts: null\ndomains:\n- domain: jhu.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/security/johns-hopkins-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Course Catalog
- News
- United States
---
