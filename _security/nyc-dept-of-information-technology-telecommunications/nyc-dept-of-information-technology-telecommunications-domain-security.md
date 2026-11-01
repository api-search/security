---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nyc.gov
  spf: true
hosts:
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: www1.nyc.gov
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nyc Dept Of Information Technology Telecommunications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NYC Dept. of Information Technology & Telecommunications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NYC Dept. of Information Technology & Telecommunications
provider_slug: nyc-dept-of-information-technology-telecommunications
slug: nyc-dept-of-information-technology-telecommunications-domain-security
source_filename: nyc-dept-of-information-technology-telecommunications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www1.nyc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: nyc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nyc-dept-of-information-technology-telecommunications/security/nyc-dept-of-information-technology-telecommunications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Technology
- NYC
- Public Services
- Information
---
