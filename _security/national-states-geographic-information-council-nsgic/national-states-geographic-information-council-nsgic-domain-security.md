---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nsgic.org
  spf: true
hosts:
- cert_expires: Jan  1 02:04:04 2027 GMT
  host: www.nsgic.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National States Geographic Information Council Nsgic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National States Geographic Information Council (NSGIC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National States Geographic Information Council (NSGIC)
provider_slug: national-states-geographic-information-council-nsgic
slug: national-states-geographic-information-council-nsgic-domain-security
source_filename: national-states-geographic-information-council-nsgic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nsgic.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 02:04:04 2027 GMT\n  hsts: false\ndomains:\n- domain: nsgic.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/national-states-geographic-information-council-nsgic/security/national-states-geographic-information-council-nsgic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geospatial
- GIS
- Government
- Standards
---
