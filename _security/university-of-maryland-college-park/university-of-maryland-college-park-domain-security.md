---
api_specs:
- filename: university-of-maryland-college-park-umdio.yaml
  format: yaml
  label: umd.io API
  slug: umdio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/openapi/university-of-maryland-college-park-umdio.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umd.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: umd.io
  spf: false
hosts:
- cert_expires: Sep 29 09:15:13 2026 GMT
  host: www.umd.edu
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 06:00:19 2026 GMT
  host: beta.umd.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 02:55:14 2026 GMT
  host: api.umd.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Maryland College Park Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Maryland College Park, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Maryland College Park
provider_slug: university-of-maryland-college-park
slug: university-of-maryland-college-park-domain-security
source_filename: university-of-maryland-college-park-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.umd.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: beta.umd.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:00:19 2026 GMT\n  hsts: false\n- host: api.umd.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 02:55:14 2026 GMT\n  hsts: false\ndomains:\n- domain: umd.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: umd.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/security/university-of-maryland-college-park-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United States
- Open Data
- Courses
- Student Run
---
