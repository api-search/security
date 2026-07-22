---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: passionfroot.me
  spf: true
hosts:
- cert_expires: Sep  2 02:59:30 2026 GMT
  host: www.passionfroot.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Passionfroot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Passionfroot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Passionfroot
provider_slug: passionfroot
slug: passionfroot-domain-security
source_filename: passionfroot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.passionfroot.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:59:30 2026 GMT\n  hsts: false\ndomains:\n- domain: passionfroot.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passionfroot/refs/heads/main/security/passionfroot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Saas
- Creator Economy
- Marketplace
- Sponsorships
- Brand Partnerships
- Payments
- AI Agent
- Go-To-Market
---
