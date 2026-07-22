---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ibasis.com
  spf: false
hosts:
- cert_expires: Sep 30 15:17:46 2026 GMT
  host: ibasis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ibasis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iBasis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: iBasis
provider_slug: ibasis
slug: ibasis-domain-security
source_filename: ibasis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ibasis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:17:46 2026 GMT\n  hsts: false\ndomains:\n- domain: ibasis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibasis/refs/heads/main/security/ibasis-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Telecom Infrastructure
- Voice
- Messaging
- IoT
- eSIM
- Roaming
- Connectivity
- MVNO
---
