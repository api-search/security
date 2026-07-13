---
api_specs:
- filename: yale-lux.yaml
  format: yaml
  label: LUX Yale Collections Discovery API
  slug: lux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-lux.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yale.edu
  spf: true
hosts:
- cert_expires: Jul 25 04:21:54 2026 GMT
  host: www.yale.edu
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 26 14:15:33 2026 GMT
  host: developers.yale.edu
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 10:15:53 2026 GMT
  host: gw.its.yale.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yale University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yale University
provider_slug: yale
slug: yale-domain-security
source_filename: yale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yale.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 04:21:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developers.yale.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:15:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: gw.its.yale.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 10:15:53 2026 GMT\n  hsts: null\ndomains:\n- domain: yale.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/security/yale-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Cultural Heritage
- Linked Data
- United States
---
