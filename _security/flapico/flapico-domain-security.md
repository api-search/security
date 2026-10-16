---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flapico.com
  spf: true
hosts:
- cert_expires: Jan  6 07:34:17 2027 GMT
  host: flapico.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flapico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flapico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flapico
provider_slug: flapico
slug: flapico-domain-security
source_filename: flapico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flapico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 07:34:17 2027 GMT\n  hsts: null\ndomains:\n- domain: flapico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flapico/refs/heads/main/security/flapico-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Infrastructure
- Web
- Lab
---
