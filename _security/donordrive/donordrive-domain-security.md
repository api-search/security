---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: donordrive.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: donordrive.com
  hsts: true
  hsts_max_age: 1200
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Donordrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DonorDrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DonorDrive
provider_slug: donordrive
slug: donordrive-domain-security
source_filename: donordrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donordrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 1200\ndomains:\n- domain: donordrive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/donordrive/security/donordrive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- Donation Platform
- SaaS
---
