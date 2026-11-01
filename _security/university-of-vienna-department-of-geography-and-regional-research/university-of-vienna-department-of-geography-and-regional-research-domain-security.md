---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: univie.ac.at
  spf: true
hosts:
- cert_expires: Apr 26 12:13:09 2027 GMT
  host: www.univie.ac.at
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Vienna Department Of Geography And Regional Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Vienna - Department of Geography and Regional Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Vienna - Department of Geography and Regional Research
provider_slug: university-of-vienna-department-of-geography-and-regional-research
slug: university-of-vienna-department-of-geography-and-regional-research-domain-security
source_filename: university-of-vienna-department-of-geography-and-regional-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.univie.ac.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 26 12:13:09 2027 GMT\n  hsts: true\n  hsts_max_age: 600\ndomains:\n- domain: univie.ac.at\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/university-of-vienna-department-of-geography-and-regional-research/security/university-of-vienna-department-of-geography-and-regional-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Geography
- Research
- Academia
- Austria
---
