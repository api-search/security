---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webloyalty.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: webloyalty.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Webloyalty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webloyalty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webloyalty
provider_slug: webloyalty
slug: webloyalty-domain-security
source_filename: webloyalty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webloyalty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: webloyalty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webloyalty/refs/heads/main/security/webloyalty-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Loyalty
- Rewards
- Ecommerce
- Customer Engagement
- Marketing
- Retail
- Cashback
---
