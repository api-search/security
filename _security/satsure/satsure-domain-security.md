---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: satsure.co
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: satsure.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Satsure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SatSure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SatSure
provider_slug: satsure
slug: satsure-domain-security
source_filename: satsure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: satsure.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: satsure.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/satsure/refs/heads/main/security/satsure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Satellite
- Artificial Intelligence
- Decision-Intelligence
- Agriculture
- Banking
---
