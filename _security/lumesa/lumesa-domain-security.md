---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumesa.ai
  spf: true
hosts:
- cert_expires: Jan 27 07:46:46 2027 GMT
  host: www.lumesa.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumesa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumesa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumesa
provider_slug: lumesa
slug: lumesa-domain-security
source_filename: lumesa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumesa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 07:46:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: lumesa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lumesa/security/lumesa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- E-commerce
- Virtual Try-On
- Fashion Tech
- Image Generation
- Company
---
