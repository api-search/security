---
api_specs:
- filename: iisc-etd-rest.yaml
  format: yaml
  label: ETD@IISc OAI-PMH
  slug: etd-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iisc/refs/heads/main/openapi/iisc-etd-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iisc.ac.in
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: iisc.ac.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: eprints.iisc.ac.in
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: etd.iisc.ac.in
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Iisc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Science Bangalore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Indian Institute of Science Bangalore
provider_slug: iisc
slug: iisc-domain-security
source_filename: iisc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iisc.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eprints.iisc.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\n- host: etd.iisc.ac.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: iisc.ac.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iisc/refs/heads/main/security/iisc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- India
---
