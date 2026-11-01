---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: panaceamedical.in
  spf: true
hosts:
- cert_expires: Apr 12 21:13:34 2027 GMT
  host: www.panaceamedical.in
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Panacea Medical Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panacea Medical Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Panacea Medical Technologies
provider_slug: panacea-medical-technologies
slug: panacea-medical-technologies-domain-security
source_filename: panacea-medical-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.panaceamedical.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 12 21:13:34 2027 GMT\n  hsts: false\ndomains:\n- domain: panaceamedical.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/panacea-medical-technologies/security/panacea-medical-technologies-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- radiotherapy
- radiology
- medical equipment
- cancer care
- manufacturing
---
