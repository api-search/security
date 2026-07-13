---
api_specs:
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Accounts API
  slug: cross-river-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River ACH Payments API
  slug: cross-river-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Wires API
  slug: cross-river-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Instant Payments API
  slug: cross-river-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Cards API
  slug: cross-river-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Lending API
  slug: cross-river-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Customer Management API
  slug: cross-river-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crossriver.com
  spf: true
  spf_record: v=spf1 include:spf.edgepilot.com include:spf.protection.outlook.com a:mail.wirexchange.goxroads.com include:mail.zendesk.com include:spf.cashedge.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crbcos.com
  spf: false
hosts:
- cert_expires: Aug 24 03:46:10 2026 GMT
  host: crossriver.com
  hsts: false
  https: true
  note: Root returns HTTP 301 (redirect to www) with no Strict-Transport-Security header observed.
  tls_version: TLSv1.3
- cert_expires: Aug 24 04:15:37 2026 GMT
  host: www.crossriver.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 02:59:58 2026 GMT
  host: docs.crossriver.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: sandbox.crbcos.com
  https: unknown
  note: The COS sandbox API host did not respond to unauthenticated HTTPS probes (no TLS handshake / HTTP response returned within timeout). Consistent with a partner-gated / access-restricted banking environment; not publicly probeable.
kind: domain-security
layout: security
method: probed
name: Cross River Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cross River, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cross River
provider_slug: cross-river
slug: cross-river-domain-security
source_filename: cross-river-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + documentation + OAuth/sandbox hosts\nhosts:\n- host: crossriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 03:46:10 2026 GMT\n  hsts: false\n  note: Root returns HTTP 301 (redirect to www) with no Strict-Transport-Security header observed.\n- host: www.crossriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:15:37 2026 GMT\n  hsts: false\n- host: docs.crossriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:59:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: sandbox.crbcos.com\n  https: unknown\n  note: >-\n    The COS sandbox API host did not respond to unauthenticated HTTPS probes\n    (no TLS handshake / HTTP response returned within timeout). Consistent with a\n    partner-gated / access-restricted banking environment; not publicly probeable.\ndomains:\n- domain: crossriver.com\n\
  \  dnssec: true\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.edgepilot.com include:spf.protection.outlook.com a:mail.wirexchange.goxroads.com include:mail.zendesk.com include:spf.cashedge.com -all'\n  dmarc: true\n  dmarc_policy: reject\n- domain: crbcos.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/security/cross-river-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Embedded Finance
- Banking as a Service
- BaaS
- Payments
- ACH
- Wire
- Push-to-Card
- Lending
- Accounts
- Cards
- Fintech
- RTP
- FedNow
---
