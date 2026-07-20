---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: everlane.com
  spf: true
hosts:
- cert_expires: Oct  5 23:32:02 2026 GMT
  host: everlane.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for everlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: everlane
provider_slug: everlane
slug: everlane-domain-security
source_filename: everlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: everlane.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlane/refs/heads/main/security/everlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fashion
- Direct-to-Consumer
- Shopify
- Agentic Commerce
---
