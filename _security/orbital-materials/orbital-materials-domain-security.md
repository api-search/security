---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbitalindustries.com
  spf: false
hosts:
- cert_expires: Oct 15 11:18:57 2026 GMT
  host: www.orbitalindustries.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Orbital Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbital Materials, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Orbital Materials
provider_slug: orbital-materials
slug: orbital-materials-domain-security
source_filename: orbital-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orbitalindustries.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 11:18:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orbitalindustries.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbital-materials/refs/heads/main/security/orbital-materials-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Materials Science
- Computational Chemistry
- Scientific Computing
- Climate Technology
- Open Source Models
- Data Centers
- Manufacturing
---
