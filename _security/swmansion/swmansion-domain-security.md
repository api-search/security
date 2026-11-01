---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: swmansion.com
  spf: true
hosts:
- cert_expires: Jan 13 08:19:35 2027 GMT
  host: swmansion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swmansion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Mansion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Software Mansion
provider_slug: swmansion
slug: swmansion-domain-security
source_filename: swmansion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swmansion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 08:19:35 2027 GMT\n  hsts: false\ndomains:\n- domain: swmansion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/swmansion/security/swmansion-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Software Development
- Mobile App
- React Native
- Elixir
---
