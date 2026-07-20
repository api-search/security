---
api_specs:
- filename: brightback-retention-openapi.yml
  format: yaml
  label: Brightback Pre-cancel API
  slug: brightback-pre-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightback/refs/heads/main/openapi/brightback-retention-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightback.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chargebee.com
  spf: true
hosts:
- host: brightback.com
  https: false
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: app.brightback.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: app.retention.chargebee.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brightback Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for brightback, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: brightback
provider_slug: brightback
slug: brightback-domain-security
source_filename: brightback-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightback.com\n  https: false\n- host: app.brightback.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\n- host: app.retention.chargebee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: brightback.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: chargebee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightback/refs/heads/main/security/brightback-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Churn Prevention
- Customer Retention
- Subscriptions
- Cancellation
- SaaS
---
