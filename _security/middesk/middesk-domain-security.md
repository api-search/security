---
api_specs:
- filename: openapi.json
  format: json
  label: Middesk Business Verification API
  slug: middesk-business-verification-api
  spec_type: OpenAPI
  url: https://docs.middesk.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: middesk.com
  spf: true
hosts:
- cert_expires: Sep 17 22:25:28 2026 GMT
  host: www.middesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:25:28 2026 GMT
  host: docs.middesk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:25:28 2026 GMT
  host: api.middesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Middesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Middesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Middesk
provider_slug: middesk
slug: middesk-domain-security
source_filename: middesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.middesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.middesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.middesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:25:28 2026 GMT\n  hsts: false\ndomains:\n- domain: middesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/middesk/refs/heads/main/security/middesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Verification
- KYB
- Know Your Business
- Identity Verification
- Compliance
- EIN Validation
- TIN Verification
- Sanctions Screening
- Business Monitoring
- Fintech
- RegTech
---
