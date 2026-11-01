---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eox.at
  spf: true
hosts:
- cert_expires: Jan 12 00:32:03 2027 GMT
  host: www.eox.at
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eox It Services Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EOX IT Services GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EOX IT Services GmbH
provider_slug: eox-it-services-gmbh
slug: eox-it-services-gmbh-domain-security
source_filename: eox-it-services-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eox.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 00:32:03 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: eox.at\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/eox-it-services-gmbh/security/eox-it-services-gmbh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- IT Services
- Cloud Solutions
- Digital Transformation
- Consulting
---
