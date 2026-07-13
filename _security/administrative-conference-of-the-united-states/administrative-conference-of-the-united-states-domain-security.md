---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acus.gov
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.acus.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: acus.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Administrative Conference Of The United States Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Administrative Conference of the United States, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Administrative Conference of the United States
provider_slug: administrative-conference-of-the-united-states
slug: administrative-conference-of-the-united-states-domain-security
source_filename: administrative-conference-of-the-united-states-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acus.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\n- host: acus.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: acus.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administrative-conference-of-the-united-states/refs/heads/main/security/administrative-conference-of-the-united-states-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Regulatory Reform
- Administrative Law
- Government Efficiency
- Open Data
- Policy Research
---
