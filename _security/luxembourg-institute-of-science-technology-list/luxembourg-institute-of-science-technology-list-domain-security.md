---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: list.lu
  spf: true
hosts:
- cert_expires: Feb  8 08:56:55 2027 GMT
  host: www.list.lu
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Luxembourg Institute Of Science Technology List Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luxembourg Institute of Science & Technology (LIST), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Luxembourg Institute of Science & Technology (LIST)
provider_slug: luxembourg-institute-of-science-technology-list
slug: luxembourg-institute-of-science-technology-list-domain-security
source_filename: luxembourg-institute-of-science-technology-list-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.list.lu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 08:56:55 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: list.lu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/luxembourg-institute-of-science-technology-list/security/luxembourg-institute-of-science-technology-list-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Research
- Innovation
- Technology
- Luxembourg
---
