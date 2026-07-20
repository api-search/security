---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allbirds.com
  spf: true
hosts:
- cert_expires: Sep  9 23:24:04 2026 GMT
  host: www.allbirds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allbirds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allbirds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allbirds
provider_slug: allbirds
slug: allbirds-domain-security
source_filename: allbirds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allbirds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:24:04 2026 GMT\n  hsts: null\ndomains:\n- domain: allbirds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allbirds/refs/heads/main/security/allbirds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Retail
- E-commerce
- Footwear
- Apparel
- Sustainability
- Direct-to-Consumer
- Agent Commerce
- Shopify
---
