---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vatit.com
  spf: true
hosts:
- cert_expires: Dec 13 17:38:13 2026 GMT
  host: vatit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vat It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VAT IT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VAT IT
provider_slug: vat-it
slug: vat-it-domain-security
source_filename: vat-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 17:38:13 2026 GMT\n  hsts: false\ndomains:\n- domain: vatit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/vat-it/security/vat-it-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Tax
- Compliance
- AI
- Finance
- SaaS
---
