---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sipgate.io
  spf: true
hosts:
- cert_expires: Jan 18 21:05:35 2027 GMT
  host: www.sipgate.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sipgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sipgate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: sipgate
provider_slug: sipgate
slug: sipgate-domain-security
source_filename: sipgate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sipgate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 21:05:35 2027 GMT\n  hsts: false\ndomains:\n- domain: sipgate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sipgate/security/sipgate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telephony
- Cloud
- API
- Communications
---
