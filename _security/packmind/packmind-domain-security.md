---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: packmind.com
  spf: true
hosts:
- cert_expires: Aug 19 15:43:51 2026 GMT
  host: packmind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packmind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Packmind
provider_slug: packmind
slug: packmind-domain-security
source_filename: packmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: packmind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packmind.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packmind/refs/heads/main/security/packmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Governance
- Code Quality
- Development Standards
---
