---
description: ''
domains:
- caa: []
  caa_lookup: timeout
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: naturalcycles.com
  spf: true
hosts:
- cert_expires: Aug 31 13:54:58 2026 GMT
  host: www.naturalcycles.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natural Cycles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natural Cycles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Natural Cycles
provider_slug: natural-cycles
slug: natural-cycles-domain-security
source_filename: natural-cycles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.naturalcycles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:54:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: naturalcycles.com\n  dnssec: false\n  caa: []\n  caa_lookup: timeout   # CAA query timed out at probe time; record not confirmed either way\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-cycles/refs/heads/main/security/natural-cycles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Tech
- Femtech
- Women's Health
- Fertility
- Birth Control
- Cycle Tracking
- Wearables
- Digital Health
- Medical Device
---
