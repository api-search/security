---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: health.gov.lk
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.hpb.health.gov.lk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covid 19 Tracker Sri Lanka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COVID-19 Tracker Sri Lanka, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: COVID-19 Tracker Sri Lanka
provider_slug: covid-19-tracker-sri-lanka
slug: covid-19-tracker-sri-lanka-domain-security
source_filename: covid-19-tracker-sri-lanka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hpb.health.gov.lk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: health.gov.lk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-19-tracker-sri-lanka/refs/heads/main/security/covid-19-tracker-sri-lanka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Public APIs
---
