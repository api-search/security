---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: twain.ai
  spf: true
hosts:
- cert_expires: Jan  5 08:00:20 2027 GMT
  host: www.twain.ai
  hsts: true
  hsts_max_age: 36000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Twain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Twain
provider_slug: twain
slug: twain-domain-security
source_filename: twain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twain.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:00:20 2027 GMT\n  hsts: true\n  hsts_max_age: 36000\ndomains:\n- domain: twain.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/twain/security/twain-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Outreach
- Sales
- Marketing
---
