---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wgicouncil.org
  spf: true
hosts:
- cert_expires: Jan 11 05:46:48 2027 GMT
  host: wgicouncil.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: World Geospatial Industry Council Wgic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Geospatial Industry Council (WGIC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: World Geospatial Industry Council (WGIC)
provider_slug: world-geospatial-industry-council-wgic
slug: world-geospatial-industry-council-wgic-domain-security
source_filename: world-geospatial-industry-council-wgic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wgicouncil.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:46:48 2027 GMT\n  hsts: false\ndomains:\n- domain: wgicouncil.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/world-geospatial-industry-council-wgic/security/world-geospatial-industry-council-wgic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- Trade Association
- Industry Council
- Membership
---
