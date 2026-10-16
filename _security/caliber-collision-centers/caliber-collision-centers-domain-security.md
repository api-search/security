---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caliber.com
  spf: true
hosts:
- cert_expires: Dec 13 13:03:05 2026 GMT
  host: www.caliber.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caliber Collision Centers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caliber Collision Centers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caliber Collision Centers
provider_slug: caliber-collision-centers
slug: caliber-collision-centers-domain-security
source_filename: caliber-collision-centers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caliber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 13:03:05 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: caliber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliber-collision-centers/refs/heads/main/security/caliber-collision-centers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Collision-Repair
- Auto-Glass
- Fleet-Services
---
