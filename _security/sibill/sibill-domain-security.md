---
api_specs:
- filename: sibill-openapi-original.json
  format: json
  label: Sibill Integration API
  slug: sibill-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/openapi/sibill-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sibill.com
  spf: true
hosts:
- cert_expires: Aug 24 19:10:56 2026 GMT
  host: sibill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:46:03 2026 GMT
  host: docs.sibill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:46:03 2026 GMT
  host: integration.sibill.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sibill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sibill, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sibill
provider_slug: sibill
slug: sibill-domain-security
source_filename: sibill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:10:56 2026 GMT\n  hsts: false\n- host: docs.sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:46:03 2026 GMT\n  hsts: false\n- host: integration.sibill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:46:03 2026 GMT\n  hsts: null\ndomains:\n- domain: sibill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sibill/refs/heads/main/security/sibill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Invoicing
- Payments
- Reconciliation
- Accounting
- Banking
- SME
- Open Banking
- Electronic Invoicing
- Italy
---
