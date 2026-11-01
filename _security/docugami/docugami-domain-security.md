---
api_specs:
- filename: docugami-openapi-generated.yml
  format: yaml
  label: Docugami API
  slug: docugami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docugami/openapi/_ae-authored/docugami-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docugami.com
  spf: true
hosts:
- cert_expires: Jan 16 09:50:05 2027 GMT
  host: www.docugami.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docugami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docugami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docugami
provider_slug: docugami
slug: docugami-domain-security
source_filename: docugami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docugami.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 09:50:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docugami.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/docugami/security/docugami-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Document Automation
- Enterprise
- Contract Management
---
