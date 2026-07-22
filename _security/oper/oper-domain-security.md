---
api_specs:
- filename: oper-api.json
  format: json
  label: Oper Connect API
  slug: oper-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-api.json
- filename: oper-resources.json
  format: json
  label: Oper Connect Resources API
  slug: oper-connect-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-resources.json
- filename: oper-metrics.json
  format: json
  label: Oper Connect Metrics API
  slug: oper-connect-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-metrics.json
- filename: oper-loan-request-webhook.json
  format: json
  label: Loan Request Webhook API
  slug: loan-request-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/openapi/oper-loan-request-webhook.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opercredits.com
  spf: true
hosts:
- cert_expires: Sep 21 19:29:12 2026 GMT
  host: www.opercredits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 15:32:59 2026 GMT
  host: developers.opercredits.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.opercredits.com
  https: false
kind: domain-security
layout: security
method: probed
name: Oper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oper, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Oper
provider_slug: oper
slug: oper-domain-security
source_filename: oper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opercredits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.opercredits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:32:59 2026 GMT\n  hsts: false\n- host: api.opercredits.com\n  https: false\ndomains:\n- domain: opercredits.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oper/refs/heads/main/security/oper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Fintech
- Mortgage
- Lending
- Loan Origination
- Digital Mortgage
- Underwriting
- Financial Services
---
