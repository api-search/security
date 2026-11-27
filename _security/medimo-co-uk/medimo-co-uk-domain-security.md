---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medimo.co.uk
  spf: true
hosts:
- cert_expires: Feb 14 00:33:46 2027 GMT
  host: medimo.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MediMo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediMo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MediMo
provider_slug: medimo-co-uk
slug: medimo-co-uk-domain-security
source_filename: medimo-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medimo.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 00:33:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medimo.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/medimo-co-uk/security/medimo-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Booking
- Physiotherapy
- United Kingdom
---
