---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fuze.com
  spf: true
hosts:
- cert_expires: Sep 20 00:45:41 2026 GMT
  host: www.fuze.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fuze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fuze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fuze
provider_slug: fuze
slug: fuze-domain-security
source_filename: fuze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fuze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:45:41 2026 GMT\n  hsts: null\ndomains:\n- domain: fuze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fuze/refs/heads/main/security/fuze-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Unified Communications
- UCaaS
- Communications
- VoIP
- Video Conferencing
- Contact Center
- Acquired
---
