---
api_specs:
- filename: charles-lindat-translation.yaml
  format: yaml
  label: LINDAT Machine Translation API
  slug: lindat-translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/openapi/charles-lindat-translation.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:tcs@cuni.cz"
  - 0 issue "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cuni.cz
  spf: true
hosts:
- cert_expires: Aug 25 11:05:25 2026 GMT
  host: www.cuni.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 14:35:48 2026 GMT
  host: dspace.cuni.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 14:35:36 2026 GMT
  host: publications.cuni.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charles University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Charles University
provider_slug: charles
slug: charles-domain-security
source_filename: charles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cuni.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:05:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dspace.cuni.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: publications.cuni.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:35:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cuni.cz\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:tcs@cuni.cz\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles/refs/heads/main/security/charles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Repository
- OAI-PMH
- Natural Language Processing
- Czechia
- Europe
---
