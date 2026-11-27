---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opus-growth.com
  spf: true
hosts:
- cert_expires: Dec 28 04:35:28 2026 GMT
  host: opus-growth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opus Growth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opus Growth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opus Growth
provider_slug: opus-growth-com
slug: opus-growth-com-domain-security
source_filename: opus-growth-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opus-growth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:35:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opus-growth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opus-growth-com/security/opus-growth-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Software-as-a-Service
- Platform
- Company
---
