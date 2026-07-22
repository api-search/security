---
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honest.com
  spf: true
hosts:
- cert_expires: Sep 13 04:23:03 2026 GMT
  host: www.honest.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Honest Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Honest Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Honest Company
provider_slug: the-honest-company
slug: the-honest-company-domain-security
source_filename: the-honest-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:23:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: honest.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-honest-company/refs/heads/main/security/the-honest-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Consumer Goods
- Ecommerce
- Retail
- Baby
- Personal Care
- Shopify
---
