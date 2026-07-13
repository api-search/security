---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stericycle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mystericycle.com
  spf: false
hosts:
- cert_expires: Sep 14 05:45:39 2026 GMT
  host: www.stericycle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:32:34 2026 GMT
  host: www.mystericycle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stericycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stericycle, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stericycle
provider_slug: stericycle
slug: stericycle-domain-security
source_filename: stericycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stericycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:45:39 2026 GMT\n  hsts: null\n- host: www.mystericycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:32:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stericycle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mystericycle.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stericycle/refs/heads/main/security/stericycle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Waste
- Compliance
- Waste Management
- Environmental Services
- Fortune 500
---
