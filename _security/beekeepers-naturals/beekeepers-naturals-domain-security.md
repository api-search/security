---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beekeepersnaturals.com
  spf: true
hosts:
- cert_expires: Sep  6 09:36:34 2026 GMT
  host: www.beekeepersnaturals.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beekeepers Naturals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beekeeper''s Naturals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beekeeper's Naturals
provider_slug: beekeepers-naturals
slug: beekeepers-naturals-domain-security
source_filename: beekeepers-naturals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beekeepersnaturals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:36:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: beekeepersnaturals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beekeepers-naturals/refs/heads/main/security/beekeepers-naturals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Consumer Packaged Goods
- Health and Wellness
- Supplements
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
---
