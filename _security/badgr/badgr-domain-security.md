---
api_specs:
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Issuers API
  slug: badgr-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr BadgeClasses API
  slug: badgr-badgeclasses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Assertions (Awarded Badges) API
  slug: badgr-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Backpack API
  slug: badgr-backpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Collections API
  slug: badgr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Users API
  slug: badgr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
- filename: badgr-openapi.yml
  format: yaml
  label: Badgr Authentication API
  slug: badgr-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/openapi/badgr-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: badgr.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: false
  dnssec: false
  domain: badgr.io
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: badgr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.badgr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.eu.badgr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Badgr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Badgr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Badgr
provider_slug: badgr
slug: badgr-domain-security
source_filename: badgr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: badgr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.badgr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eu.badgr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: badgr.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: badgr.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"\
  amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/badgr/refs/heads/main/security/badgr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Badges
- Open Badges
- Micro-Credentials
- Credentialing
- Verifiable Credentials
- Education
- Open Source
---
