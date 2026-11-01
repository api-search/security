---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: klimadatastyrelsen.dk
  spf: true
hosts:
- cert_expires: Jan 21 23:07:22 2027 GMT
  host: eng.klimadatastyrelsen.dk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Danish Agency For Climate Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Danish Agency for Climate Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Danish Agency for Climate Data
provider_slug: the-danish-agency-for-climate-data
slug: the-danish-agency-for-climate-data-domain-security
source_filename: the-danish-agency-for-climate-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eng.klimadatastyrelsen.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:07:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: klimadatastyrelsen.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/the-danish-agency-for-climate-data/security/the-danish-agency-for-climate-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate
- Data
- Denmark
- Government
- Environment
---
