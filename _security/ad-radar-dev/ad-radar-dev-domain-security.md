---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ad-radar.dev
  spf: true
hosts:
- cert_expires: Dec 29 12:45:48 2026 GMT
  host: ad-radar.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ad Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ad Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ad Radar
provider_slug: ad-radar-dev
slug: ad-radar-dev-domain-security
source_filename: ad-radar-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ad-radar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 12:45:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ad-radar.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ad-radar-dev/security/ad-radar-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Marketing
- Artificial Intelligence
- Competitive Intelligence
- Social Media
---
