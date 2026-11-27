---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nuboohub.com
  spf: true
hosts:
- cert_expires: Jan  2 07:46:03 2027 GMT
  host: nuboohub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nuboo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuboo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nuboo
provider_slug: nuboohub-com
slug: nuboohub-com-domain-security
source_filename: nuboohub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuboohub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 07:46:03 2027 GMT\n  hsts: false\ndomains:\n- domain: nuboohub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nuboohub-com/security/nuboohub-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- ERP
- CRM
- Payments
- Integration
---
