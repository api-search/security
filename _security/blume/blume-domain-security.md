---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blume.com
  spf: true
hosts:
- cert_expires: Aug 26 05:21:03 2026 GMT
  host: blume.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blume, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blume
provider_slug: blume
slug: blume-domain-security
source_filename: blume-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blume.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: blume.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blume/refs/heads/main/security/blume-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Skincare
- Beauty
- Self-Care
- E-commerce
- Consumer
- Shopify
- Agent Commerce
- Universal Commerce Protocol
- MCP
---
