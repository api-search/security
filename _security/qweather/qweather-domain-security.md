---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qweather.com
  spf: true
hosts:
- cert_expires: Sep 24 11:11:20 2026 GMT
  host: dev.qweather.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QWeather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QWeather
provider_slug: qweather
slug: qweather-domain-security
source_filename: qweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.qweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 11:11:20 2026 GMT\n  hsts: false\ndomains:\n- domain: qweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qweather/refs/heads/main/security/qweather-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Public APIs
---
