---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: usekojo.com
  spf: true
hosts:
- cert_expires: Sep 13 00:43:59 2026 GMT
  host: usekojo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kojo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kojo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kojo
provider_slug: kojo
slug: kojo-domain-security
source_filename: kojo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usekojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:43:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usekojo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kojo/refs/heads/main/security/kojo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Procurement
- Materials Management
- Supply Chain
- Contractors
- ERP Integration
- EDI
- Inventory
- Construction Technology
---
