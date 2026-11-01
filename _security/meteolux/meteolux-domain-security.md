---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: meteolux.lu
  spf: true
hosts:
- cert_expires: Feb  6 14:09:55 2027 GMT
  host: meteolux.lu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meteolux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeteoLux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MeteoLux
provider_slug: meteolux
slug: meteolux-domain-security
source_filename: meteolux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meteolux.lu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 14:09:55 2027 GMT\n  hsts: false\ndomains:\n- domain: meteolux.lu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/meteolux/security/meteolux-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Weather
- Forecast
- Climate
- Luxembourg
- Europe
---
