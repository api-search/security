---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: explorationmaps.com
  spf: false
hosts:
- cert_expires: Jan  2 07:21:42 2027 GMT
  host: explorationmaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exploration Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exploration Maps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Exploration Maps
provider_slug: explorationmaps-com
slug: explorationmaps-com-domain-security
source_filename: explorationmaps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: explorationmaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 07:21:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: explorationmaps.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/explorationmaps-com/security/explorationmaps-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Mining
- GIS
- Mapping
- Exploration
- Junior Mining
---
