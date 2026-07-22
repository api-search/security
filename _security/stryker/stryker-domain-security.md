---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stryker.com
  spf: true
hosts:
- cert_expires: Nov 21 10:51:30 2026 GMT
  host: www.stryker.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stryker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stryker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stryker
provider_slug: stryker
slug: stryker-domain-security
source_filename: stryker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stryker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 10:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stryker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stryker/refs/heads/main/security/stryker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical Devices
- Healthcare Technology
- Fortune 500
- Medical Equipment
- Orthopedics
- Surgical Equipment
---
