---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terraco2.com
  spf: true
hosts:
- cert_expires: Nov 22 08:14:41 2026 GMT
  host: terraco2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terra Co2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terra CO2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Terra CO2
provider_slug: terra-co2
slug: terra-co2-domain-security
source_filename: terra-co2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terraco2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 08:14:41 2026 GMT\n  hsts: false\ndomains:\n- domain: terraco2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-co2/refs/heads/main/security/terra-co2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Building Materials
- Construction
- Cement
- Concrete
- Climate Tech
- Carbon Reduction
- Sustainability
- Manufacturing
- Materials Science
---
