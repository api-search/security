---
api_specs:
- filename: avo-app-openapi-generated.yml
  format: yaml
  label: Avo API
  slug: avo-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avo-app/openapi/_ae-authored/avo-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avo.app
  spf: true
hosts:
- cert_expires: Jan 19 00:48:11 2027 GMT
  host: www.avo.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avo App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avo
provider_slug: avo-app
slug: avo-app-domain-security
source_filename: avo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 00:48:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: avo.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/avo-app/security/avo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Governance
- Analytics
- AI
- SaaS
---
