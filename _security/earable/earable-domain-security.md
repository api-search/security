---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frenzband.com
  spf: true
hosts:
- cert_expires: Sep  9 18:41:34 2026 GMT
  host: frenzband.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Earable
provider_slug: earable
slug: earable-domain-security
source_filename: earable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frenzband.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:41:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: frenzband.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earable/refs/heads/main/security/earable-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wearables
- Sleep Technology
- Neuroscience
- Health
- Consumer Electronics
- Agentic Commerce
- Shopify
---
