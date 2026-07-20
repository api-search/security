---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apptopia.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: apptopia.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apptopia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apptopia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apptopia
provider_slug: apptopia
slug: apptopia-domain-security
source_filename: apptopia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apptopia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: apptopia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptopia/refs/heads/main/security/apptopia-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Mobile
- App Store Intelligence
- Market Intelligence
- Alternative Data
- Analytics
- Consumer Insights
- Advertising
---
