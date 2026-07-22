---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: himarley.com
  spf: true
hosts:
- cert_expires: Sep 15 02:53:09 2026 GMT
  host: www.himarley.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hi Marley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hi Marley, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hi Marley
provider_slug: hi-marley
slug: hi-marley-domain-security
source_filename: hi-marley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.himarley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:53:09 2026 GMT\n  hsts: false\ndomains:\n- domain: himarley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hi-marley/refs/heads/main/security/hi-marley-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance Tech
- Insurance
- Claims
- Messaging
- SMS
- Conversational AI
- Property and Casualty
- Customer Communications
- FNOL
---
