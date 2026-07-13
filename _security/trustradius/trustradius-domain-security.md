---
api_specs:
- filename: trustradius-public-openapi.yml
  format: yaml
  label: TrustRadius Public API
  slug: trustradius-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-public-openapi.yml
- filename: trustradius-reviews-openapi.yml
  format: yaml
  label: TrustRadius Reviews API
  slug: trustradius-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-reviews-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trustradius.com
  spf: true
hosts:
- cert_expires: Aug 23 02:31:08 2026 GMT
  host: www.trustradius.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:19:24 2026 GMT
  host: solutions.trustradius.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:33:11 2026 GMT
  host: apidocs.trustradius.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustradius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustRadius, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TrustRadius
provider_slug: trustradius
slug: trustradius-domain-security
source_filename: trustradius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trustradius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:31:08 2026 GMT\n  hsts: null\n- host: solutions.trustradius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:19:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.trustradius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:33:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trustradius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/security/trustradius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B Software Reviews
- Buyer Intelligence
- Intent Data
- Software Reviews
- Reviews
- Product Reviews
- Categories
---
