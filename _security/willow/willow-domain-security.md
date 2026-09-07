---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onewillow.com
  spf: true
hosts:
- cert_expires: Nov  5 05:07:02 2026 GMT
  host: onewillow.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Willow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Willow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Willow
provider_slug: willow
slug: willow-domain-security
source_filename: willow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onewillow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:07:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: onewillow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willow/refs/heads/main/security/willow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Health
- Breast Pumps
- Maternal Health
- Medical Devices
- Ecommerce
- Agentic Commerce
- MCP
- UCP
- agent-native
- Shopify
---
