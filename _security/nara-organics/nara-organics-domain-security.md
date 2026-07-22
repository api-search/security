---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nara.com
  spf: true
hosts:
- cert_expires: Sep  8 23:46:31 2026 GMT
  host: nara.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nara Organics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nara Organics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nara Organics
provider_slug: nara-organics
slug: nara-organics-domain-security
source_filename: nara-organics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: nara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nara-organics/refs/heads/main/security/nara-organics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Commerce
- Retail
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Infant Formula
---
