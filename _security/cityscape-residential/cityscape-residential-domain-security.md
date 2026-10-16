---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cityscaperesidential.com
  spf: true
hosts:
- cert_expires: Nov 20 10:49:01 2026 GMT
  host: cityscaperesidential.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cityscape Residential Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cityscape Residential, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cityscape Residential
provider_slug: cityscape-residential
slug: cityscape-residential-domain-security
source_filename: cityscape-residential-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cityscaperesidential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 10:49:01 2026 GMT\n  hsts: false\ndomains:\n- domain: cityscaperesidential.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityscape-residential/refs/heads/main/security/cityscape-residential-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Development
- Multifamily
- Investment
---
