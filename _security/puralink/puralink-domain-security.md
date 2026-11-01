---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: puralink.com.au
  spf: true
hosts:
- cert_expires: Jan 13 05:48:09 2027 GMT
  host: www.puralink.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Puralink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puralink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Puralink
provider_slug: puralink
slug: puralink-domain-security
source_filename: puralink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.puralink.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 05:48:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: puralink.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/puralink/security/puralink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- pipe inspection
- autonomous robots
- infrastructure
- robotics
- wastewater
- oil & gas
- mining
- data center
---
