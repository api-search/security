---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: understoryweather.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: understoryweather.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Understory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Understory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Understory
provider_slug: understory
slug: understory-domain-security
source_filename: understory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: understoryweather.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: understoryweather.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/understory/refs/heads/main/security/understory-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Insurance
- InsurTech
- Weather
- Parametric Insurance
- Sensors
---
