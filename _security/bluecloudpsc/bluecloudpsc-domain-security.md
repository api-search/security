---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bluecloudpsc.com
  spf: true
hosts:
- cert_expires: Jul 24 23:59:59 2026 GMT
  host: bluecloudpsc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluecloudpsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Cloud Pediatric Surgery Centers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blue Cloud Pediatric Surgery Centers
provider_slug: bluecloudpsc
slug: bluecloudpsc-domain-security
source_filename: bluecloudpsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluecloudpsc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bluecloudpsc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecloudpsc/refs/heads/main/security/bluecloudpsc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pediatric
- Dental
- Oral Surgery
- Ambulatory Surgery Center
- Anesthesia
---
