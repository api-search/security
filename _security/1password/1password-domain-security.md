---
api_specs:
- filename: 1password-accounts-api-openapi.yml
  format: yaml
  label: 1Password Accounts API
  slug: 1password-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-accounts-api-openapi.yml
- filename: 1password-activity-api-openapi.yml
  format: yaml
  label: 1Password Activity API
  slug: 1password-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-activity-api-openapi.yml
- filename: 1password-audit-events-api-openapi.yml
  format: yaml
  label: 1Password Audit Events API
  slug: 1password-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-audit-events-api-openapi.yml
- filename: 1password-files-api-openapi.yml
  format: yaml
  label: 1Password Files API
  slug: 1password-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-files-api-openapi.yml
- filename: 1password-health-api-openapi.yml
  format: yaml
  label: 1Password Health API
  slug: 1password-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-health-api-openapi.yml
- filename: 1password-introspection-api-openapi.yml
  format: yaml
  label: 1Password Introspection API
  slug: 1password-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-introspection-api-openapi.yml
- filename: 1password-item-usages-api-openapi.yml
  format: yaml
  label: 1Password Item Usages API
  slug: 1password-item-usages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-item-usages-api-openapi.yml
- filename: 1password-items-api-openapi.yml
  format: yaml
  label: 1Password Items API
  slug: 1password-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-items-api-openapi.yml
- filename: 1password-metrics-api-openapi.yml
  format: yaml
  label: 1Password Metrics API
  slug: 1password-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-metrics-api-openapi.yml
- filename: 1password-sign-in-attempts-api-openapi.yml
  format: yaml
  label: 1Password Sign-In Attempts API
  slug: 1password-sign-in-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-sign-in-attempts-api-openapi.yml
- filename: 1password-vaults-api-openapi.yml
  format: yaml
  label: 1Password Vaults API
  slug: 1password-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/openapi/1password-vaults-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:alerts+caa@agilebits.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1password.com
  spf: true
hosts:
- cert_expires: Sep 26 13:45:15 2026 GMT
  host: 1password.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: developer.1password.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: events.1password.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Password Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Password, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1Password
provider_slug: 1password
slug: 1password-domain-security
source_filename: 1password-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1password.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:45:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.1password.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: events.1password.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 1password.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:alerts+caa@agilebits.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/security/1password-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Password Manager
- Passwords
- Security
- Secrets
---
