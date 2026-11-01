---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: concordia.ca
  spf: true
hosts:
- cert_expires: Mar 22 19:16:29 2027 GMT
  host: www.concordia.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Concordia University Montr Al Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concordia University Montréal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Concordia University Montréal
provider_slug: concordia-university-montr-al
slug: concordia-university-montr-al-domain-security
source_filename: concordia-university-montr-al-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concordia.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 19:16:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: concordia.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/concordia-university-montr-al/security/concordia-university-montr-al-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Education
- Canada
- Montreal
- HigherEducation
- Company
---
