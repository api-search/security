---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virtuix.com
  spf: true
hosts:
- cert_expires: Nov 25 05:43:01 2026 GMT
  host: virtuix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Virtuix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtuix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Virtuix
provider_slug: virtuix
slug: virtuix-domain-security
source_filename: virtuix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtuix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 05:43:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virtuix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuix/refs/heads/main/security/virtuix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Virtual Reality
- Gaming
- Hardware
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Esports
- Game Development
- Location Based Entertainment
- Consumer Electronics
---
