---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icanhazepoch.com
  spf: false
hosts:
- cert_expires: Jul 29 20:16:50 2026 GMT
  host: icanhazepoch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icanhazepoch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Icanhazepoch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Icanhazepoch
provider_slug: icanhazepoch
slug: icanhazepoch-domain-security
source_filename: icanhazepoch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icanhazepoch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 20:16:50 2026 GMT\n  hsts: false\ndomains:\n- domain: icanhazepoch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icanhazepoch/refs/heads/main/security/icanhazepoch-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
