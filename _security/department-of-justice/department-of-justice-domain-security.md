---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: justice.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foia.gov
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.justice.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.foia.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: bjs.ojp.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of Justice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Justice, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Justice
provider_slug: department-of-justice
slug: department-of-justice-domain-security
source_filename: department-of-justice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.justice.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.foia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bjs.ojp.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: justice.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: foia.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-justice/refs/heads/main/security/department-of-justice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bureau of Justice Statistics
- Crime
- Federal Government
- FOIA
- Justice
- News
- Open Data
- Press Releases
- Statistics
---
