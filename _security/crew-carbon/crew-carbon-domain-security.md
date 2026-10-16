---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: crewcarbon.com
  spf: true
hosts:
- cert_expires: Jan  7 13:19:54 2027 GMT
  host: crewcarbon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crew Carbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CREW Carbon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: CREW Carbon
provider_slug: crew-carbon
slug: crew-carbon-domain-security
source_filename: crew-carbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crewcarbon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 13:19:54 2027 GMT\n  hsts: false\ndomains:\n- domain: crewcarbon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crew-carbon/refs/heads/main/security/crew-carbon-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Wastewater Treatment
- Carbon Removal
- Process Intensification
- Alkalinity Enhancement
- Industrial Water
---
