---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: traileraddict.com
  spf: false
hosts:
- cert_expires: Jul 30 21:26:43 2026 GMT
  host: www.traileraddict.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Traileraddict Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrailerAddict, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TrailerAddict
provider_slug: traileraddict
slug: traileraddict-domain-security
source_filename: traileraddict-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traileraddict.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 21:26:43 2026 GMT\n  hsts: false\ndomains:\n- domain: traileraddict.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traileraddict/refs/heads/main/security/traileraddict-domain-security.yml
summary_line: TLSv1.3
tags:
- Video
- Public APIs
---
