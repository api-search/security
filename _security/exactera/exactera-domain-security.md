---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exactera.com
  spf: true
hosts:
- cert_expires: Sep 22 06:04:32 2026 GMT
  host: exactera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exactera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exactera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exactera
provider_slug: exactera
slug: exactera-domain-security
source_filename: exactera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exactera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:04:32 2026 GMT\n  hsts: false\ndomains:\n- domain: exactera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactera/refs/heads/main/security/exactera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Tax
- Tax Technology
- Transfer Pricing
- Tax Compliance
- Regulatory Compliance
- Financial Services
- R&D Tax Credits
- SaaS
---
