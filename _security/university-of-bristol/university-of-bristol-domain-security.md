---
api_specs:
- filename: openapi.json
  format: json
  label: Bristol Research Portal (Pure) API
  slug: pure-research-api
  spec_type: OpenAPI
  url: https://research-information.bris.ac.uk/ws/api/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bristol.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bris.ac.uk
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.bristol.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 17:20:09 2026 GMT
  host: research-information.bris.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: data.bris.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Bristol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bristol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Bristol
provider_slug: university-of-bristol
slug: university-of-bristol-domain-security
source_filename: university-of-bristol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bristol.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: research-information.bris.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: data.bris.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bristol.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bris.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/security/university-of-bristol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United Kingdom
---
