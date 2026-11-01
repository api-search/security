---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sgligis.com
  spf: true
hosts:
- cert_expires: Jan 15 09:43:51 2027 GMT
  host: www.sgligis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sgl Resources Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SGL Resources Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SGL Resources Limited
provider_slug: sgl-resources-limited
slug: sgl-resources-limited-domain-security
source_filename: sgl-resources-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sgligis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 09:43:51 2027 GMT\n  hsts: false\ndomains:\n- domain: sgligis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sgl-resources-limited/security/sgl-resources-limited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- GIS
- Mapping
- CAD
- Software
---
