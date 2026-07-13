---
api_specs:
- filename: trustpilot-business-units-openapi.yml
  format: yaml
  label: Trustpilot Business Units API
  slug: trustpilot-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-business-units-openapi.yml
- filename: trustpilot-service-reviews-openapi.yml
  format: yaml
  label: Trustpilot Service Reviews API
  slug: trustpilot-service-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-service-reviews-openapi.yml
- filename: trustpilot-invitation-openapi.yml
  format: yaml
  label: Trustpilot Invitation API
  slug: trustpilot-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-invitation-openapi.yml
- filename: trustpilot-product-reviews-openapi.yml
  format: yaml
  label: Trustpilot Product Reviews API
  slug: trustpilot-product-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/openapi/trustpilot-product-reviews-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trustpilot.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.trustpilot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: developers.trustpilot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.trustpilot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustpilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trustpilot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trustpilot
provider_slug: trustpilot
slug: trustpilot-domain-security
source_filename: trustpilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trustpilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\n- host: developers.trustpilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.trustpilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trustpilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustpilot/refs/heads/main/security/trustpilot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consumer Reviews
- Reviews
- Trust
- Ratings
- Business Profiles
- Product Reviews
---
