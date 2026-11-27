---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extreme-media.co.uk
  spf: true
hosts:
- cert_expires: Jan 26 14:30:50 2027 GMT
  host: extreme-media.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Extreme Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extreme Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extreme Media
provider_slug: extreme-media-co-uk
slug: extreme-media-co-uk-domain-security
source_filename: extreme-media-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extreme-media.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 14:30:50 2027 GMT\n  hsts: false\ndomains:\n- domain: extreme-media.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/extreme-media-co-uk/security/extreme-media-co-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- Software-as-a-Service
- Web App
- Garmin
---
