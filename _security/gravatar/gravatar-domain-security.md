---
api_specs:
- filename: openapi
  format: yaml
  label: Gravatar Avatar API
  slug: avatar-api
  spec_type: OpenAPI
  url: https://api.gravatar.com/v3/openapi
- filename: openapi
  format: yaml
  label: Gravatar REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.gravatar.com/v3/openapi
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gravatar.com
  spf: true
hosts:
- cert_expires: Sep 20 22:48:57 2026 GMT
  host: docs.gravatar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 19:43:59 2026 GMT
  host: 0.gravatar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 19:43:59 2026 GMT
  host: api.gravatar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gravatar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravatar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gravatar
provider_slug: gravatar
slug: gravatar-domain-security
source_filename: gravatar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.gravatar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:48:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 0.gravatar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:43:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gravatar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:43:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gravatar.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/security/gravatar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Avatars
- Identity
- Profiles
- Social
- Images
- GraphQL
- REST
---
