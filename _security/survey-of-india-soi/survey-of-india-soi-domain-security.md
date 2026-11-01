---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: surveyofindia.gov.in
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.surveyofindia.gov.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Survey Of India Soi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Survey of India (SoI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Survey of India (SoI)
provider_slug: survey-of-india-soi
slug: survey-of-india-soi-domain-security
source_filename: survey-of-india-soi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.surveyofindia.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: surveyofindia.gov.in\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/survey-of-india-soi/security/survey-of-india-soi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
