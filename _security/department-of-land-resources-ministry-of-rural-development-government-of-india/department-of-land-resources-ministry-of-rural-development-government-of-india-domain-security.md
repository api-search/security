---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dolr.gov.in
  spf: true
hosts:
- cert_expires: Jan 11 12:25:35 2027 GMT
  host: www.dolr.gov.in
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Department Of Land Resources Ministry Of Rural Development Government Of India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Land Resources, Ministry of Rural Development, Government of India, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Department of Land Resources, Ministry of Rural Development, Government of India
provider_slug: department-of-land-resources-ministry-of-rural-development-government-of-india
slug: department-of-land-resources-ministry-of-rural-development-government-of-india-domain-security
source_filename: department-of-land-resources-ministry-of-rural-development-government-of-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dolr.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 12:25:35 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: dolr.gov.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/department-of-land-resources-ministry-of-rural-development-government-of-india/security/department-of-land-resources-ministry-of-rural-development-government-of-india-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
