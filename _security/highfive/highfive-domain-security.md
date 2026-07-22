---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: highfive.com
  spf: true
hosts:
- cert_expires: Jan 21 01:33:26 2027 GMT
  host: highfive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highfive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highfive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Highfive
provider_slug: highfive
slug: highfive-domain-security
source_filename: highfive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highfive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 01:33:26 2027 GMT\n  hsts: null\ndomains:\n- domain: highfive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highfive/refs/heads/main/security/highfive-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Enterprise
- Video Conferencing
- Collaboration
- Acquired
- Dialpad
---
