---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: strata.io
  spf: true
hosts:
- cert_expires: Oct 11 21:00:40 2026 GMT
  host: strata.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:56:15 2026 GMT
  host: docs.strata.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 17:01:36 2026 GMT
  host: auth.us-east-2.strata.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strata Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strata Identity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Strata Identity
provider_slug: strata-identity
slug: strata-identity-domain-security
source_filename: strata-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:00:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.strata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:56:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth.us-east-2.strata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:01:36 2026 GMT\n  hsts: null\ndomains:\n- domain: strata.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strata-identity/refs/heads/main/security/strata-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity
- Identity Orchestration
- Authentication
- Authorization
- Single Sign-On
- IAM
- OAuth
- SAML
- OpenID Connect
- AI Identity
- Security
---
