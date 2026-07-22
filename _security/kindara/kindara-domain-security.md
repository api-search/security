---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kindara.com
  spf: true
hosts:
- cert_expires: Aug 19 13:01:09 2026 GMT
  host: kindara.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kindara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kindara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kindara
provider_slug: kindara
slug: kindara-domain-security
source_filename: kindara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kindara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 13:01:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kindara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kindara/refs/heads/main/security/kindara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fertility
- Femtech
- Reproductive Health
- Women's Health
- Menstrual Cycle Tracking
- Health
- Mobile App
---
