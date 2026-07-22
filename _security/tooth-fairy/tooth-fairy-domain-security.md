---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toothfairyapp.co.uk
  spf: true
hosts:
- cert_expires: Aug 29 00:40:25 2026 GMT
  host: toothfairyapp.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tooth Fairy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tooth Fairy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tooth Fairy
provider_slug: tooth-fairy
slug: tooth-fairy-domain-security
source_filename: tooth-fairy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toothfairyapp.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:40:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: toothfairyapp.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooth-fairy/refs/heads/main/security/tooth-fairy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Dental
- Telehealth
- Healthcare
- Orthodontics
- Mobile App
- United Kingdom
---
