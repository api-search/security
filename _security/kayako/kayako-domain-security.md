---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kayako.com
  spf: true
hosts:
- cert_expires: Dec  1 18:15:11 2026 GMT
  host: kayako.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kayako Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kayako, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kayako
provider_slug: kayako
slug: kayako-domain-security
source_filename: kayako-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kayako.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 18:15:11 2026 GMT\n  hsts: false\ndomains:\n- domain: kayako.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kayako/security/kayako-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Support
- AI
- SaaS
- Help Desk
---
