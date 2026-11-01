---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gc.ca
  spf: true
hosts:
- cert_expires: Apr 30 23:59:59 2027 GMT
  host: www.charts.gc.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fisheries And Oceans Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fisheries and Oceans Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fisheries and Oceans Canada
provider_slug: fisheries-and-oceans-canada
slug: fisheries-and-oceans-canada-domain-security
source_filename: fisheries-and-oceans-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charts.gc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fisheries-and-oceans-canada/security/fisheries-and-oceans-canada-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- Fisheries
- Marine
- Environment
- Government
- Fisheries
- Marine
- Environment
---
