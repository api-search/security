---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: binotel.ua
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: www.binotel.ua
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Binotel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binotel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Binotel
provider_slug: binotel
slug: binotel-domain-security
source_filename: binotel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.binotel.ua\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: binotel.ua\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/binotel/security/binotel-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Telephony
- Cloud
- Business
- Communications
---
