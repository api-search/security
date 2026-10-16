---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upsales.com
  spf: true
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: upsales.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Upsales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upsales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Upsales
provider_slug: upsales
slug: upsales-domain-security
source_filename: upsales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upsales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: upsales.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsales/refs/heads/main/security/upsales-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sales
- AI
- CRM
- SaaS
---
