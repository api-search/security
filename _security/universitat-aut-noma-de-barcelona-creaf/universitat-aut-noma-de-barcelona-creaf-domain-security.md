---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: creaf.cat
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.creaf.cat
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Universitat Aut Noma De Barcelona Creaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universitat Autònoma de Barcelona (CREAF), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Universitat Autònoma de Barcelona (CREAF)
provider_slug: universitat-aut-noma-de-barcelona-creaf
slug: universitat-aut-noma-de-barcelona-creaf-domain-security
source_filename: universitat-aut-noma-de-barcelona-creaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creaf.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: creaf.cat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/universitat-aut-noma-de-barcelona-creaf/security/universitat-aut-noma-de-barcelona-creaf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Ecology
- Environment
- Data
---
