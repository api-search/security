---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: covidtracking.com
  spf: true
hosts:
- cert_expires: Aug 26 21:57:40 2026 GMT
  host: covidtracking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covid Tracking Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covid Tracking Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Covid Tracking Project
provider_slug: covid-tracking-project
slug: covid-tracking-project-domain-security
source_filename: covid-tracking-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covidtracking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:57:40 2026 GMT\n  hsts: false\ndomains:\n- domain: covidtracking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-tracking-project/refs/heads/main/security/covid-tracking-project-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Public APIs
---
