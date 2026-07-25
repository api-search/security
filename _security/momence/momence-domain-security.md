---
api_specs:
- filename: momence-auth-api-openapi.yml
  format: yaml
  label: Momence auth API
  slug: momence-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-auth-api-openapi.yml
- filename: momence-host-api-openapi.yml
  format: yaml
  label: Momence host API
  slug: momence-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-host-api-openapi.yml
- filename: momence-host-checkout-api-openapi.yml
  format: yaml
  label: Momence host-checkout API
  slug: momence-host-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-host-checkout-api-openapi.yml
- filename: momence-member-addresses-api-openapi.yml
  format: yaml
  label: Momence member-addresses API
  slug: momence-member-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-addresses-api-openapi.yml
- filename: momence-member-api-openapi.yml
  format: yaml
  label: Momence member API
  slug: momence-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-api-openapi.yml
- filename: momence-member-checkout-api-openapi.yml
  format: yaml
  label: Momence member-checkout API
  slug: momence-member-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-checkout-api-openapi.yml
- filename: momence-member-host-api-openapi.yml
  format: yaml
  label: Momence member-host API
  slug: momence-member-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-host-api-openapi.yml
- filename: momence-member-sessions-api-openapi.yml
  format: yaml
  label: Momence member-sessions API
  slug: momence-member-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: momence.com
  spf: true
hosts:
- cert_expires: Sep 29 21:29:17 2026 GMT
  host: momence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:57:03 2026 GMT
  host: api.docs.momence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:29:17 2026 GMT
  host: api.momence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Momence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Momence, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Momence
provider_slug: momence
slug: momence-domain-security
source_filename: momence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: momence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:29:17 2026 GMT\n  hsts: false\n- host: api.docs.momence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:57:03 2026 GMT\n  hsts: null\n- host: api.momence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:29:17 2026 GMT\n  hsts: null\ndomains:\n- domain: momence.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/security/momence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Wellness
- Studio Management
- Booking
- Scheduling
- Memberships
- Payments
- Class Management
---
