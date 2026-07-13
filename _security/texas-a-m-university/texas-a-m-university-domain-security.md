---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tamu.edu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tamus.edu
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.tamu.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: geoservices.tamu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 15:53:37 2026 GMT
  host: it.tamus.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Texas A M University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Texas A&M University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Texas A&M University
provider_slug: texas-a-m-university
slug: texas-a-m-university-domain-security
source_filename: texas-a-m-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tamu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: geoservices.tamu.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: it.tamus.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:53:37 2026 GMT\n  hsts: false\ndomains:\n- domain: tamu.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tamus.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/security/texas-a-m-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Geocoding
- Library
- United States
---
