---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flocore.tech
  spf: true
hosts:
- cert_expires: Jan  4 08:35:05 2027 GMT
  host: flocore.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FLOCORE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLOCORE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FLOCORE
provider_slug: flocore-tech
slug: flocore-tech-domain-security
source_filename: flocore-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flocore.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 08:35:05 2027 GMT\n  hsts: false\ndomains:\n- domain: flocore.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flocore-tech/security/flocore-tech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- ERP
- OperationalControl
- Ontology
- MicroModels
---
