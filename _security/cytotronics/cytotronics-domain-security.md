---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cytotronics.com
  spf: true
hosts:
- cert_expires: Jan 18 05:24:11 2027 GMT
  host: cytotronics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cytotronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CytoTronics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CytoTronics
provider_slug: cytotronics
slug: cytotronics-domain-security
source_filename: cytotronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cytotronics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 05:24:11 2027 GMT\n  hsts: false\ndomains:\n- domain: cytotronics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cytotronics/security/cytotronics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biotechnology
- Cell Biology
- Electrophysiology
- Drug Discovery
- Phenotypic Screening
---
