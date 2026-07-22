---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agrostar.in
  spf: true
hosts:
- cert_expires: Sep 26 07:07:21 2026 GMT
  host: corporate.agrostar.in
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agrostar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrostar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agrostar
provider_slug: agrostar
slug: agrostar-domain-security
source_filename: agrostar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.agrostar.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:07:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: agrostar.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrostar/refs/heads/main/security/agrostar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Agriculture
- AgriTech
- Farming
- India
- Farmer Advisory
- Agri Inputs
- Marketplace
---
