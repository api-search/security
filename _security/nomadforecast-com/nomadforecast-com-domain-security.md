---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomadforecast.com
  spf: true
hosts:
- cert_expires: Jan 22 08:00:31 2027 GMT
  host: nomadforecast.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomad Forecast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomad Forecast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nomad Forecast
provider_slug: nomadforecast-com
slug: nomadforecast-com-domain-security
source_filename: nomadforecast-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomadforecast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 08:00:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: nomadforecast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nomadforecast-com/security/nomadforecast-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Family
- Travel
- Planning
- Artificial Intelligence
- Privacy
---
