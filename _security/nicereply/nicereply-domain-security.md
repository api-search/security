---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nicereply.com
  spf: true
hosts:
- cert_expires: Oct  1 16:40:40 2026 GMT
  host: www.nicereply.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 16:45:11 2026 GMT
  host: api.nicereply.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nicereply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nicereply, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nicereply
provider_slug: nicereply
slug: nicereply-domain-security
source_filename: nicereply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nicereply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:40:40 2026 GMT\n  hsts: false\n- host: api.nicereply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:45:11 2026 GMT\n  hsts: null\ndomains:\n- domain: nicereply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nicereply/refs/heads/main/security/nicereply-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Satisfaction
- CSAT
- CES
- NPS
- Surveys
- Helpdesk
- Customer Experience
---
