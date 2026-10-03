---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: babyquip.com
  spf: true
hosts:
- cert_expires: Nov 10 11:15:58 2026 GMT
  host: www.babyquip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Babyquip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BabyQuip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BabyQuip
provider_slug: babyquip
slug: babyquip-domain-security
source_filename: babyquip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.babyquip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 11:15:58 2026 GMT\n  hsts: false\ndomains:\n- domain: babyquip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babyquip/refs/heads/main/security/babyquip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- BabyGear
- Rentals
- Marketplace
- Travel
- Family
---
