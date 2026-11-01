---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umd.edu
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: geog.umd.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Maryland Dept Of Geographical Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Maryland Dept. of Geographical Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Maryland Dept. of Geographical Sciences
provider_slug: university-of-maryland-dept-of-geographical-sciences
slug: university-of-maryland-dept-of-geographical-sciences-domain-security
source_filename: university-of-maryland-dept-of-geographical-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geog.umd.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: umd.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/university-of-maryland-dept-of-geographical-sciences/security/university-of-maryland-dept-of-geographical-sciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Geography
- Research
- GIS
- Remote Sensing
---
