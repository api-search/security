---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instant.so
  spf: true
hosts:
- cert_expires: Sep 25 15:02:10 2026 GMT
  host: instant.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instant Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instant Commerce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instant Commerce
provider_slug: instant-commerce
slug: instant-commerce-domain-security
source_filename: instant-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instant.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instant.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instant-commerce/refs/heads/main/security/instant-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Enterprise Software
- Ecommerce
- Shopify
- No Code
- Page Builder
- Artificial Intelligence
- AI Agents
- Conversion Rate Optimization
- Developer Tools
---
