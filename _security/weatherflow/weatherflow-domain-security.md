---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tempestwx.com
  spf: false
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: tempestwx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Weatherflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeatherFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WeatherFlow
provider_slug: weatherflow
slug: weatherflow-domain-security
source_filename: weatherflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tempestwx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tempestwx.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/weatherflow/security/weatherflow-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Weather
- API
- IoT
- Real-time
---
