---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beautypie.com
  spf: true
hosts:
- cert_expires: Sep 29 03:49:33 2026 GMT
  host: www.beautypie.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beauty Pie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beauty Pie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beauty Pie
provider_slug: beauty-pie
slug: beauty-pie-domain-security
source_filename: beauty-pie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beautypie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:49:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: beautypie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beauty-pie/refs/heads/main/security/beauty-pie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Beauty
- Cosmetics
- Skincare
- Retail
- E-Commerce
- Shopify
- Agentic Commerce
---
