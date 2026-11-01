---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oascities.org
  spf: true
hosts:
- cert_expires: Jan  2 16:36:47 2027 GMT
  host: oascities.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Agile Smart Cities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open & Agile Smart Cities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open & Agile Smart Cities
provider_slug: open-agile-smart-cities
slug: open-agile-smart-cities-domain-security
source_filename: open-agile-smart-cities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oascities.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 16:36:47 2027 GMT\n  hsts: false\ndomains:\n- domain: oascities.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/open-agile-smart-cities/security/open-agile-smart-cities-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Smart Cities
- Interoperability
- Digital Innovation
- Artificial Intelligence
- Digital Sovereignty
---
