---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opendtu.solar
  spf: false
hosts:
- cert_expires: Dec 20 05:51:21 2026 GMT
  host: www.opendtu.solar
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opendtu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenDTU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenDTU
provider_slug: opendtu
slug: opendtu-domain-security
source_filename: opendtu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendtu.solar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 05:51:21 2026 GMT\n  hsts: false\ndomains:\n- domain: opendtu.solar\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opendtu/security/opendtu-domain-security.yml
summary_line: TLSv1.3
tags:
- solar
- firmware
- open-source
- iot
- energy-monitoring
---
