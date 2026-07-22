---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vaya.so
  spf: true
hosts:
- cert_expires: Oct  4 18:00:48 2026 GMT
  host: vaya.so
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vaya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Vaya
provider_slug: vaya
slug: vaya-domain-security
source_filename: vaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vaya.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:00:48 2026 GMT\n  hsts: false\ndomains:\n- domain: vaya.so\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaya/refs/heads/main/security/vaya-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI
- Astrology
- Vedic Astrology
- Consultations
- Consumer Apps
- India
---
