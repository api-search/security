---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rheaply.com
  spf: true
hosts:
- cert_expires: Sep 30 13:51:40 2026 GMT
  host: rheaply.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rheaply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rheaply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rheaply
provider_slug: rheaply
slug: rheaply-domain-security
source_filename: rheaply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rheaply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:51:40 2026 GMT\n  hsts: false\ndomains:\n- domain: rheaply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rheaply/refs/heads/main/security/rheaply-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Circular Economy
- Sustainability
- Asset Management
- Inventory Management
- Reuse Marketplace
- Decommissioning
- ESG
---
