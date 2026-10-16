---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: copcomm.com
  spf: true
hosts:
- cert_expires: Dec 12 14:51:14 2026 GMT
  host: copcomm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Copincommunications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copincommunications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Copincommunications
provider_slug: copincommunications
slug: copincommunications-domain-security
source_filename: copincommunications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: copcomm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 14:51:14 2026 GMT\n  hsts: false\ndomains:\n- domain: copcomm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copincommunications/refs/heads/main/security/copincommunications-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Print
- DirectMail
- Personalization
---
