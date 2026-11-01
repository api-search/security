---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chghealthcare.com
  spf: true
hosts:
- cert_expires: Jan  3 21:31:47 2027 GMT
  host: chghealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chg Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHG Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CHG Healthcare
provider_slug: chg-healthcare
slug: chg-healthcare-domain-security
source_filename: chg-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chghealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:31:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chghealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chg-healthcare/security/chg-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Staffing
- Physician
- Technology
---
