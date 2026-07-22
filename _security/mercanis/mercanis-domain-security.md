---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mercanis.com
  spf: true
hosts:
- cert_expires: Aug 24 20:26:50 2026 GMT
  host: www.mercanis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercanis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercanis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mercanis
provider_slug: mercanis
slug: mercanis-domain-security
source_filename: mercanis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mercanis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:26:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mercanis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercanis/refs/heads/main/security/mercanis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Applicative Saas
- Procurement
- Sourcing
- Supplier Management
- Contract Management
- Spend Analytics
- Source-to-Contract
- AI Agents
---
