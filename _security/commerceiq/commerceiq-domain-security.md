---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commerceiq.ai
  spf: true
hosts:
- cert_expires: Oct  1 10:53:47 2026 GMT
  host: www.commerceiq.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commerceiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CommerceIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CommerceIQ
provider_slug: commerceiq
slug: commerceiq-domain-security
source_filename: commerceiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commerceiq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commerceiq.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerceiq/refs/heads/main/security/commerceiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Retail Media
- Digital Shelf
- Artificial Intelligence
- Retail
- Analytics
- Marketing
---
