---
api_specs:
- filename: wildapricot-admin-api-openapi.yml
  format: yaml
  label: WildApricot Admin API
  slug: wildapricot-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/openapi/wildapricot-admin-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:abuse@wildapricot.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wildapricot.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wildapricot.org
  spf: true
hosts:
- cert_expires: Oct  2 21:55:27 2026 GMT
  host: www.wildapricot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: app.wildapricot.com
  https: false
- cert_expires: Oct  6 15:53:34 2026 GMT
  host: api.wildapricot.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wildapricot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WildApricot, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WildApricot
provider_slug: wildapricot
slug: wildapricot-domain-security
source_filename: wildapricot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wildapricot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:55:27 2026 GMT\n  hsts: false\n- host: app.wildapricot.com\n  https: false\n- host: api.wildapricot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:53:34 2026 GMT\n  hsts: null\ndomains:\n- domain: wildapricot.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:abuse@wildapricot.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wildapricot.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/security/wildapricot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Membership Management
- Associations
- Nonprofit
- Events
- Payments
---
