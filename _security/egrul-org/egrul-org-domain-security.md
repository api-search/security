---
api_specs:
- filename: egrul-org-openapi-generated.yml
  format: yaml
  label: egrul-org API
  slug: egrul-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/egrul-org/openapi/_ae-authored/egrul-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: egrul.org
  spf: true
hosts:
- cert_expires: Dec 15 23:21:15 2026 GMT
  host: egrul.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Egrul Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for egrul-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: egrul-org
provider_slug: egrul-org
slug: egrul-org-domain-security
source_filename: egrul-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: egrul.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:21:15 2026 GMT\n  hsts: false\ndomains:\n- domain: egrul.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/egrul-org/security/egrul-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Government
- Data
- Russia
---
