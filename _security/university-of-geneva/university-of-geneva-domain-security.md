---
api_specs:
- filename: university-of-geneva-yareta.yaml
  format: yaml
  label: Yareta Research Data API
  slug: yareta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/openapi/university-of-geneva-yareta.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unige.ch
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.unige.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 13:26:53 2026 GMT
  host: archive-ouverte.unige.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 05:30:00 2026 GMT
  host: yareta.unige.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Geneva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Geneva, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Geneva
provider_slug: university-of-geneva
slug: university-of-geneva-domain-security
source_filename: university-of-geneva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unige.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: archive-ouverte.unige.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:26:53 2026 GMT\n  hsts: false\n- host: yareta.unige.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:30:00 2026 GMT\n  hsts: false\ndomains:\n- domain: unige.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/security/university-of-geneva-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Science
- Research Data
- Institutional Repository
- Switzerland
- Europe
---
