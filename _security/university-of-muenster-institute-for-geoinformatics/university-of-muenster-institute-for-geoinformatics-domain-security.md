---
description: ''
domains:
- caa:
  - 0 issue "pki.dfn.de"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:ca@uni-muenster.de"
  - 0 issuemail "pki.dfn.de"
  - 0 issue "telesec.de"
  - 0 issuemail "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uni-muenster.de
  spf: true
hosts:
- cert_expires: Mar 17 20:16:28 2027 GMT
  host: ifgi.uni-muenster.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Muenster Institute For Geoinformatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Muenster - Institute for Geoinformatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Muenster - Institute for Geoinformatics
provider_slug: university-of-muenster-institute-for-geoinformatics
slug: university-of-muenster-institute-for-geoinformatics-domain-security
source_filename: university-of-muenster-institute-for-geoinformatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ifgi.uni-muenster.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 20:16:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: uni-muenster.de\n  dnssec: false\n  caa:\n  - 0 issue \"pki.dfn.de\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:ca@uni-muenster.de\"\n  - 0 issuemail \"pki.dfn.de\"\n  - 0 issue \"telesec.de\"\n  - 0 issuemail \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/university-of-muenster-institute-for-geoinformatics/security/university-of-muenster-institute-for-geoinformatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geoinformatics
- Research
- GIS
- University
- Germany
---
