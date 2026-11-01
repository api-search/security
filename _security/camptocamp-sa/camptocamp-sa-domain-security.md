---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: camptocamp.com
  spf: true
hosts:
- cert_expires: Jan 18 08:24:15 2027 GMT
  host: www.camptocamp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Camptocamp Sa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camptocamp SA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Camptocamp SA
provider_slug: camptocamp-sa
slug: camptocamp-sa-domain-security
source_filename: camptocamp-sa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.camptocamp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 08:24:15 2027 GMT\n  hsts: false\ndomains:\n- domain: camptocamp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/camptocamp-sa/security/camptocamp-sa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- GIS
- OpenSource
- Consulting
- Geospatial
- Mapping
---
