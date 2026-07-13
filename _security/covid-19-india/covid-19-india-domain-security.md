---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: covid19india.org
  spf: true
hosts:
- cert_expires: Sep 22 23:44:21 2026 GMT
  host: data.covid19india.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covid 19 India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covid-19 India, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Covid-19 India
provider_slug: covid-19-india
slug: covid-19-india-domain-security
source_filename: covid-19-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.covid19india.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:44:21 2026 GMT\n  hsts: false\ndomains:\n- domain: covid19india.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-19-india/refs/heads/main/security/covid-19-india-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Public APIs
---
