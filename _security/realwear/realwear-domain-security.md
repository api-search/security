---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realwear.com
  spf: true
hosts:
- cert_expires: Oct  5 15:02:03 2026 GMT
  host: www.realwear.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realwear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealWear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RealWear
provider_slug: realwear
slug: realwear-domain-security
source_filename: realwear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realwear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: realwear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realwear/refs/heads/main/security/realwear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Wearables
- Voice AI
- Augmented Reality
- Assisted Reality
- Frontline Workers
- Industrial
- Android
- Hands-Free
---
