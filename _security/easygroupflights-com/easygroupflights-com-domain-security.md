---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: easygroupflights.com
  spf: true
hosts:
- cert_expires: Jan 22 11:46:57 2027 GMT
  host: easygroupflights.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EasyGroupFlights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyGroupFlights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EasyGroupFlights
provider_slug: easygroupflights-com
slug: easygroupflights-com-domain-security
source_filename: easygroupflights-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easygroupflights.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:46:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: easygroupflights.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/easygroupflights-com/security/easygroupflights-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- GroupFlights
- B2B
- Aviation
- Europe
---
