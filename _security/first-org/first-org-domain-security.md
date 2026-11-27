---
api_specs:
- filename: first-org-openapi-generated.yml
  format: yaml
  label: FIRST API
  slug: first-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/first-org/openapi/_ae-authored/first-org-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:caa@first.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: first.org
  spf: true
hosts:
- cert_expires: Dec 26 16:13:04 2026 GMT
  host: first.org
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FIRST Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIRST, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FIRST
provider_slug: first-org
slug: first-org-domain-security
source_filename: first-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: first.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:13:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: first.org\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:caa@first.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/first-org/security/first-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Community
- Standards
- Training
- Non-Profit
---
