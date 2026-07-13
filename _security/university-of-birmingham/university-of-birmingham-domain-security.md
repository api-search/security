---
api_specs:
- filename: university-of-birmingham-english-constructicon.yaml
  format: yaml
  label: English Constructicon API
  slug: english-constructicon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-birmingham/refs/heads/main/openapi/university-of-birmingham-english-constructicon.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: birmingham.ac.uk
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bham.ac.uk
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.birmingham.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: edata.bham.ac.uk
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: etheses.bham.ac.uk
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Birmingham Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Birmingham, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: University of Birmingham
provider_slug: university-of-birmingham
slug: university-of-birmingham-domain-security
source_filename: university-of-birmingham-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.birmingham.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: edata.bham.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: etheses.bham.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: birmingham.ac.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: bham.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-birmingham/refs/heads/main/security/university-of-birmingham-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research
- Open Data
- Library
- OAI-PMH
---
