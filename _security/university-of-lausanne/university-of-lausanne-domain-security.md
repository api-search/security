---
api_specs:
- filename: university-of-lausanne-spica.yaml
  format: yaml
  label: SPICA Atlas API
  slug: spica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-spica.yaml
- filename: university-of-lausanne-iris.yaml
  format: yaml
  label: IRIS Repository (DSpace REST API)
  slug: iris
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/openapi/university-of-lausanne-iris.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unil.ch
  spf: true
hosts:
- cert_expires: Aug 25 23:07:37 2026 GMT
  host: www.unil.ch
  hsts: true
  hsts_max_age: 32140800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 06:52:30 2026 GMT
  host: spica.unil.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 06:52:30 2026 GMT
  host: iris.unil.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Lausanne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Lausanne, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Lausanne
provider_slug: university-of-lausanne
slug: university-of-lausanne-domain-security
source_filename: university-of-lausanne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unil.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:07:37 2026 GMT\n  hsts: true\n  hsts_max_age: 32140800\n- host: spica.unil.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:52:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: iris.unil.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:52:30 2026 GMT\n  hsts: false\ndomains:\n- domain: unil.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lausanne/refs/heads/main/security/university-of-lausanne-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Switzerland
- Open Science
- Research Data
- Institutional Repository
---
