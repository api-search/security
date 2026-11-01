---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openwb.de
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: openwb.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openwb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openWB (self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: openWB (self-hosted)
provider_slug: openwb
slug: openwb-domain-security
source_filename: openwb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openwb.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: openwb.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openwb/security/openwb-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- EVCharging
- SmartHome
- OpenSource
- SelfHosted
---
