---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: postcron.com
  spf: true
hosts:
- cert_expires: Jan 16 11:16:30 2027 GMT
  host: postcron.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Socialtools Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for postcron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: postcron
provider_slug: socialtools-me
slug: socialtools-me-domain-security
source_filename: socialtools-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postcron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:16:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: postcron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/socialtools-me/security/socialtools-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Scheduling
- Marketing
- Automation
- Postcron
---
