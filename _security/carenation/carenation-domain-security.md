---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carenation.in
  spf: false
hosts:
- cert_expires: Dec 13 03:32:27 2026 GMT
  host: carenation.in
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carenation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carenation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Carenation
provider_slug: carenation
slug: carenation-domain-security
source_filename: carenation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carenation.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 03:32:27 2026 GMT\n  hsts: false\ndomains:\n- domain: carenation.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carenation/refs/heads/main/security/carenation-domain-security.yml
summary_line: TLSv1.2
tags:
- Telehealth
- Healthcare
- RemoteCare
- Digital Health
- Platform
---
