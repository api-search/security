---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: electra.earth
  spf: true
hosts:
- cert_expires: Oct 18 23:19:10 2026 GMT
  host: www.electra.earth
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Electra
provider_slug: electra
slug: electra-domain-security
source_filename: electra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.electra.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:19:10 2026 GMT\n  hsts: null\ndomains:\n- domain: electra.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electra/refs/heads/main/security/electra-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Clean Energy
- Climate Tech
- Industrial
- Manufacturing
- Materials
- Iron
- Steel
- Decarbonization
- Electrochemistry
- Mining
---
