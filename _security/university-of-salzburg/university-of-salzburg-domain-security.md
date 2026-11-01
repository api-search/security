---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zgis.at
  spf: true
hosts:
- cert_expires: Mar  4 10:07:36 2027 GMT
  host: www.zgis.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Salzburg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Salzburg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: University of Salzburg
provider_slug: university-of-salzburg
slug: university-of-salzburg-domain-security
source_filename: university-of-salzburg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zgis.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 10:07:36 2027 GMT\n  hsts: false\ndomains:\n- domain: zgis.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/university-of-salzburg/security/university-of-salzburg-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- Research
- Austria
- University
---
