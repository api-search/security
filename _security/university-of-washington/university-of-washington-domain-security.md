---
api_specs:
- filename: index.html
  format: yaml
  label: Student Web Service (SWS)
  slug: student-web-service
  spec_type: OpenAPI
  url: https://ws.admin.washington.edu/student/swagger/index.html
- filename: index.html
  format: yaml
  label: IdCard Web Service
  slug: idcard-web-service
  spec_type: OpenAPI
  url: https://ws.admin.washington.edu/idcard/swagger/index.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: washington.edu
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.washington.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: webservices.washington.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: ws.admin.washington.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Washington Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Washington, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Washington
provider_slug: university-of-washington
slug: university-of-washington-domain-security
source_filename: university-of-washington-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.washington.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\n- host: webservices.washington.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: ws.admin.washington.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: washington.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-washington/refs/heads/main/security/university-of-washington-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United States
- Student Information
- Identity
- Library
- Open Data
---
