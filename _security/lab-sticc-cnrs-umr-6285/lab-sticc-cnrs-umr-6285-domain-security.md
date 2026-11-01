---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lab-sticc.fr
  spf: true
hosts:
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: www.lab-sticc.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lab Sticc Cnrs Umr 6285 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lab-STICC CNRS UMR 6285, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lab-STICC CNRS UMR 6285
provider_slug: lab-sticc-cnrs-umr-6285
slug: lab-sticc-cnrs-umr-6285-domain-security
source_filename: lab-sticc-cnrs-umr-6285-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lab-sticc.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lab-sticc.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lab-sticc-cnrs-umr-6285/security/lab-sticc-cnrs-umr-6285-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Research
- Laboratory
- CNRS
- InformationTechnology
- France
---
