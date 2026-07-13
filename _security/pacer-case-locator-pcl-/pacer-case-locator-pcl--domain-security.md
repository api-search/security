---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uscourts.gov
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: pacer.uscourts.gov
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pacer Case Locator Pcl  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PACER Case Locator (PCL), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PACER Case Locator (PCL)
provider_slug: pacer-case-locator-pcl-
slug: pacer-case-locator-pcl--domain-security
source_filename: pacer-case-locator-pcl--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pacer.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: uscourts.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pacer-case-locator-pcl-/refs/heads/main/security/pacer-case-locator-pcl--domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Courts
- Federal Cases
- Government
- Legal
---
