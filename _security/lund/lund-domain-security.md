---
api_specs:
- filename: lund-lup-search.yaml
  format: yaml
  label: Lund University Publications (LUP) Search API
  slug: lup-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lund/refs/heads/main/openapi/lund-lup-search.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lu.se
  spf: true
hosts:
- cert_expires: Aug 18 07:07:01 2026 GMT
  host: www.lunduniversity.lu.se
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 26 11:48:25 2026 GMT
  host: lup.lub.lu.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:42:15 2026 GMT
  host: portal.research.lu.se
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lund University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lund University
provider_slug: lund
slug: lund-domain-security
source_filename: lund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunduniversity.lu.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 07:07:01 2026 GMT\n  hsts: false\n- host: lup.lub.lu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:48:25 2026 GMT\n  hsts: false\n- host: portal.research.lu.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: lu.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lund/refs/heads/main/security/lund-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Sweden
- Research
- Library
- Open Data
- Publications
---
