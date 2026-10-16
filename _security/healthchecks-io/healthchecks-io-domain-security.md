---
api_specs:
- filename: healthchecks-io-openapi-generated.yml
  format: yaml
  label: Healthchecks.io API
  slug: healthchecks-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/healthchecks-io/refs/heads/main/openapi/_ae-authored/healthchecks-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: healthchecks.io
  spf: true
hosts:
- cert_expires: Apr 17 23:59:59 2027 GMT
  host: healthchecks.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Healthchecks Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healthchecks.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Healthchecks.io
provider_slug: healthchecks-io
slug: healthchecks-io-domain-security
source_filename: healthchecks-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healthchecks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: healthchecks.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthchecks-io/refs/heads/main/security/healthchecks-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Cron
- DevOps
- OpenSource
- SaaS
---
