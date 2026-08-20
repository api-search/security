---
api_specs:
- filename: paymentsense-connect-v2.json
  format: json
  label: Paymentsense Connect REST API
  slug: connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-connect-v2.json
- filename: paymentsense-connect-e-v0.json
  format: json
  label: Paymentsense Connect-E REST API
  slug: connect-e-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/openapi/paymentsense-connect-e-v0.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paymentsense.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paymentsense.cloud
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.paymentsense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:20:57 2026 GMT
  host: docs.connect.paymentsense.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: your-host-here.connect.paymentsense.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paymentsense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paymentsense, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paymentsense
provider_slug: paymentsense
slug: paymentsense-domain-security
source_filename: paymentsense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paymentsense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\n- host: docs.connect.paymentsense.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:20:57 2026 GMT\n  hsts: false\n- host: your-host-here.connect.paymentsense.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paymentsense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: paymentsense.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymentsense/refs/heads/main/security/paymentsense-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Card Payments
- Acquiring
- Point-of-Sale
- In-Person Payments
---
