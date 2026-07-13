---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: covid19tracker.ca
  spf: false
hosts:
- cert_expires: Sep  2 09:11:15 2026 GMT
  host: api.covid19tracker.ca
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Covid 19 Tracker Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COVID-19 Tracker Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: COVID-19 Tracker Canada
provider_slug: covid-19-tracker-canada
slug: covid-19-tracker-canada-domain-security
source_filename: covid-19-tracker-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.covid19tracker.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 09:11:15 2026 GMT\n  hsts: false\ndomains:\n- domain: covid19tracker.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-19-tracker-canada/refs/heads/main/security/covid-19-tracker-canada-domain-security.yml
summary_line: TLSv1.2
tags:
- Health
- Public APIs
---
