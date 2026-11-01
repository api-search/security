---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hft-stuttgart.de
  spf: true
hosts:
- cert_expires: Jan 18 09:21:38 2027 GMT
  host: www.hft-stuttgart.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hochschule F R Technik Stuttgart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hochschule für Technik Stuttgart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hochschule für Technik Stuttgart
provider_slug: hochschule-f-r-technik-stuttgart
slug: hochschule-f-r-technik-stuttgart-domain-security
source_filename: hochschule-f-r-technik-stuttgart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hft-stuttgart.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 09:21:38 2027 GMT\n  hsts: false\ndomains:\n- domain: hft-stuttgart.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hochschule-f-r-technik-stuttgart/security/hochschule-f-r-technik-stuttgart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- University
- Engineering
- Computer Science
- Research
---
