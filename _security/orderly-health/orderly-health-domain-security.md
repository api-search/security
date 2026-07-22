---
api_specs:
- filename: orderly-health-provider-directory-openapi.json
  format: json
  label: Orderly Provider Directory API
  slug: orderly-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderly-health/refs/heads/main/openapi/orderly-health-provider-directory-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: orderlyhealth.com
  spf: true
hosts:
- cert_expires: Sep 28 10:29:08 2026 GMT
  host: orderlyhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:50:24 2026 GMT
  host: api.orderlyhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orderly Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orderly Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Orderly Health
provider_slug: orderly-health
slug: orderly-health-domain-security
source_filename: orderly-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orderlyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:29:08 2026 GMT\n  hsts: false\n- host: api.orderlyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:50:24 2026 GMT\n  hsts: null\ndomains:\n- domain: orderlyhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderly-health/refs/heads/main/security/orderly-health-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Provider Data
- Provider Directory
- Health Data
- Machine Learning
- Data Quality
- Interoperability
---
