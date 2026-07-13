---
api_specs:
- filename: openapi
  format: yaml
  label: PHAIDRA REST API
  slug: phaidra-api
  spec_type: OpenAPI
  url: https://services.phaidra.univie.ac.at/api/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: univie.ac.at
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: phaidra.org
  spf: true
hosts:
- cert_expires: Jan  4 14:17:49 2027 GMT
  host: www.univie.ac.at
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 15 11:15:03 2026 GMT
  host: phaidra.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 18:11:55 2026 GMT
  host: services.phaidra.univie.ac.at
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Vienna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Vienna, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Vienna
provider_slug: university-of-vienna
slug: university-of-vienna-domain-security
source_filename: university-of-vienna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.univie.ac.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:17:49 2027 GMT\n  hsts: true\n  hsts_max_age: 600\n- host: phaidra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 15 11:15:03 2026 GMT\n  hsts: false\n- host: services.phaidra.univie.ac.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 18:11:55 2026 GMT\n  hsts: false\ndomains:\n- domain: univie.ac.at\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: phaidra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/security/university-of-vienna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Repository
- Open Data
- Austria
- Europe
---
