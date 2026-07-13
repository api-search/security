---
api_specs:
- filename: uc-davis-peaks.yaml
  format: yaml
  label: CAES PEAKS API
  slug: peaks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-peaks.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucdavis.edu
  spf: true
hosts:
- cert_expires: Sep  5 13:27:19 2026 GMT
  host: www.ucdavis.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: iet-ws.ucdavis.edu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: health.ucdavis.edu
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uc Davis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Davis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of California, Davis
provider_slug: uc-davis
slug: uc-davis-domain-security
source_filename: uc-davis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucdavis.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:27:19 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: iet-ws.ucdavis.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: health.ucdavis.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: ucdavis.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/security/uc-davis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United States
- California
- Identity
- Health
---
