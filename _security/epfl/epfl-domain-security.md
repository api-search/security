---
api_specs:
- filename: epfl-actu.yaml
  format: yaml
  label: EPFL Actu News API
  slug: actu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-actu.yaml
- filename: epfl-memento.yaml
  format: yaml
  label: EPFL Memento Events API
  slug: memento
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-memento.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epfl.ch
  spf: true
hosts:
- cert_expires: Aug 14 12:58:47 2026 GMT
  host: www.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:32:22 2026 GMT
  host: actu.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:41:00 2026 GMT
  host: memento.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epfl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPFL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EPFL
provider_slug: epfl
slug: epfl-domain-security
source_filename: epfl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 12:58:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: actu.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: memento.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:41:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epfl.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/security/epfl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Switzerland
- Europe
---
