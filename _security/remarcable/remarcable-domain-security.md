---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remarcable.com
  spf: true
hosts:
- cert_expires: Sep 25 05:51:46 2026 GMT
  host: www.remarcable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remarcable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remarcable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Remarcable
provider_slug: remarcable
slug: remarcable-domain-security
source_filename: remarcable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remarcable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: remarcable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remarcable/refs/heads/main/security/remarcable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Procurement
- Materials Management
- Supply Chain
- Electrical Contractors
- MEP
- Inventory
- ERP Integration
- Prefabrication
- Tool Management
- Construction Technology
---
