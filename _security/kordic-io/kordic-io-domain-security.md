---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kordic.io
  spf: true
hosts:
- cert_expires: Jan 14 18:05:12 2027 GMT
  host: kordic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kordic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kordic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kordic
provider_slug: kordic-io
slug: kordic-io-domain-security
source_filename: kordic-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kordic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 18:05:12 2027 GMT\n  hsts: false\ndomains:\n- domain: kordic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kordic-io/security/kordic-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Sales Pipeline
- Invoicing
- Payment Tracking
- WhatsApp Integration
- AI Pre‑call Briefing
- Mobile App
- Integration
---
