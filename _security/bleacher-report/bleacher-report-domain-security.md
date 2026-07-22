---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bleacherreport.com
  spf: true
hosts:
- cert_expires: Sep  3 01:42:07 2026 GMT
  host: bleacherreport.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bleacher Report Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bleacher Report, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bleacher Report
provider_slug: bleacher-report
slug: bleacher-report-domain-security
source_filename: bleacher-report-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bleacherreport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:42:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: bleacherreport.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bleacher-report/refs/heads/main/security/bleacher-report-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Media
- Sports News
- Content
- Entertainment
---
