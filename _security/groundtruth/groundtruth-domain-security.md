---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: groundtruth.com
  spf: true
hosts:
- cert_expires: Sep 30 11:19:44 2026 GMT
  host: www.groundtruth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groundtruth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GroundTruth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GroundTruth
provider_slug: groundtruth
slug: groundtruth-domain-security
source_filename: groundtruth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groundtruth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:19:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: groundtruth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/security/groundtruth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Advertising
- Location Intelligence
- Marketing
- Adtech
- Location-Based Marketing
---
