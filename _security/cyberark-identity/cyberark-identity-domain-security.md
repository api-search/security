---
api_specs:
- filename: cyberark-identity-openapi.yml
  format: yaml
  label: CyberArk Identity API
  slug: identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cyberark.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cyberark.cloud
  spf: true
hosts:
- cert_expires: Sep 18 14:43:50 2026 GMT
  host: www.cyberark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:43:50 2026 GMT
  host: api-docs-identity.cyberark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <tenant>.id.cyberark.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Cyberark Identity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyberArk Identity, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CyberArk Identity
provider_slug: cyberark-identity
slug: cyberark-identity-domain-security
source_filename: cyberark-identity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cyberark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs-identity.cyberark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <tenant>.id.cyberark.cloud\n  https: false\ndomains:\n- domain: cyberark.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cyberark.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/security/cyberark-identity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity
- Access Management
- IAM
- Single Sign-On
- SSO
- Multi-Factor Authentication
- OAuth
- Zero Trust
---
