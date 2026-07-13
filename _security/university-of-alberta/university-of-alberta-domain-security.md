---
api_specs:
- filename: university-of-alberta-borealis-dataverse.yaml
  format: yaml
  label: University of Alberta Research Data (Borealis Dataverse) API
  slug: borealis-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-alberta/refs/heads/main/openapi/university-of-alberta-borealis-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ualberta.ca
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: borealisdata.ca
  spf: true
hosts:
- cert_expires: Dec 12 12:46:16 2026 GMT
  host: www.ualberta.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: borealisdata.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Alberta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Alberta, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Alberta
provider_slug: university-of-alberta
slug: university-of-alberta-domain-security
source_filename: university-of-alberta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ualberta.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 12:46:16 2026 GMT\n  hsts: null\n- host: borealisdata.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ualberta.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: borealisdata.ca\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-alberta/refs/heads/main/security/university-of-alberta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Library
- Canada
---
