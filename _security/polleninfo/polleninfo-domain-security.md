---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: polleninformation.eu
  spf: false
hosts:
- cert_expires: Jan 25 06:42:30 2027 GMT
  host: polleninformation.eu
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polleninfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polleninfo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Polleninfo
provider_slug: polleninfo
slug: polleninfo-domain-security
source_filename: polleninfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polleninformation.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 06:42:30 2027 GMT\n  hsts: false\ndomains:\n- domain: polleninformation.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/polleninfo/security/polleninfo-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Health
- Allergy
- Data
- Europe
---
