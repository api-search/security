---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: modretro.com
  spf: true
hosts:
- cert_expires: Nov  6 05:44:32 2026 GMT
  host: modretro.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modretro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModRetro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ModRetro
provider_slug: modretro
slug: modretro-domain-security
source_filename: modretro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modretro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 05:44:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: modretro.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modretro/refs/heads/main/security/modretro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer Electronics
- Gaming
- Retro Gaming
- Hardware
- E-Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Open Source Hardware
---
