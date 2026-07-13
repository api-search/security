---
api_specs:
- filename: stockholm-figshare.yaml
  format: yaml
  label: Stockholm University Research Data Repository (Figshare)
  slug: figshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockholm/refs/heads/main/openapi/stockholm-figshare.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: su.se
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: diva-portal.org
  spf: false
hosts:
- cert_expires: Oct 27 15:22:29 2026 GMT
  host: www.su.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:19:57 2026 GMT
  host: su.diva-portal.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: su.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stockholm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockholm University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stockholm University
provider_slug: stockholm
slug: stockholm-domain-security
source_filename: stockholm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.su.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 15:22:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: su.diva-portal.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:19:57 2026 GMT\n  hsts: false\n- host: su.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: su.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: diva-portal.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockholm/refs/heads/main/security/stockholm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Sweden
- Europe
---
