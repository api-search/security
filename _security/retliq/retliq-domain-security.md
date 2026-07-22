---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: retliq.com
  spf: true
hosts:
- cert_expires: Oct  9 15:09:46 2026 GMT
  host: retliq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retliq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RetLiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RetLiq
provider_slug: retliq
slug: retliq-domain-security
source_filename: retliq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:09:46 2026 GMT\n  hsts: false\ndomains:\n- domain: retliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retliq/refs/heads/main/security/retliq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
