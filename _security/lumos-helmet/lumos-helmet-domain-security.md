---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lumoshelmet.co
  spf: true
hosts:
- cert_expires: Aug 30 16:01:02 2026 GMT
  host: lumoshelmet.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumos Helmet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumos Helmet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lumos Helmet
provider_slug: lumos-helmet
slug: lumos-helmet-domain-security
source_filename: lumos-helmet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumoshelmet.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 16:01:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: lumoshelmet.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos-helmet/refs/heads/main/security/lumos-helmet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer Hardware
- Wearables
- Cycling
- Bike Safety
- Smart Helmets
- IoT
- Mobile Apps
---
