---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voyagertechnologies.com
  spf: true
hosts:
- cert_expires: Nov 26 02:49:13 2026 GMT
  host: voyagertechnologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voyager Space Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyager Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voyager Technologies
provider_slug: voyager-space-holdings
slug: voyager-space-holdings-domain-security
source_filename: voyager-space-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyagertechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 02:49:13 2026 GMT\n  hsts: false\ndomains:\n- domain: voyagertechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyager-space-holdings/refs/heads/main/security/voyager-space-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Space
- Defense
- Aerospace
- Propulsion
- Satellite
- Lunar
- Space Stations
- Public Company
---
