---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savagex.com
  spf: true
hosts:
- cert_expires: Nov  2 04:59:48 2026 GMT
  host: www.savagex.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: 'HSTS observed directly on the response headers of https://www.savagex.com/ (a Cloudflare bot-challenge 403, cf-mitigated: challenge). Edge is Cloudflare; origin is TechStyle.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savage X Fenty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savage X Fenty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Savage X Fenty
provider_slug: savage-x-fenty
slug: savage-x-fenty-domain-security
source_filename: savage-x-fenty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.savagex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 04:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: >-\n    HSTS observed directly on the response headers of https://www.savagex.com/ (a Cloudflare\n    bot-challenge 403, cf-mitigated: challenge). Edge is Cloudflare; origin is TechStyle.\ndomains:\n- domain: savagex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savage-x-fenty/refs/heads/main/security/savage-x-fenty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Apparel
- Lingerie
- Retail
- E-commerce
- Direct to Consumer
- Subscription
---
