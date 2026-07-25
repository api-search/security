---
api_specs:
- filename: accredible-analytics-api-openapi.yml
  format: yaml
  label: Accredible Analytics API
  slug: accredible-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-analytics-api-openapi.yml
- filename: accredible-credentials-api-openapi.yml
  format: yaml
  label: Accredible Credentials API
  slug: accredible-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-credentials-api-openapi.yml
- filename: accredible-departments-api-openapi.yml
  format: yaml
  label: Accredible Departments API
  slug: accredible-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-departments-api-openapi.yml
- filename: accredible-designs-api-openapi.yml
  format: yaml
  label: Accredible Designs API
  slug: accredible-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-designs-api-openapi.yml
- filename: accredible-evidence-items-api-openapi.yml
  format: yaml
  label: Accredible Evidence Items API
  slug: accredible-evidence-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-evidence-items-api-openapi.yml
- filename: accredible-groups-api-openapi.yml
  format: yaml
  label: Accredible Groups API
  slug: accredible-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-groups-api-openapi.yml
- filename: accredible-issuer-api-openapi.yml
  format: yaml
  label: Accredible Issuer API
  slug: accredible-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-issuer-api-openapi.yml
- filename: accredible-references-api-openapi.yml
  format: yaml
  label: Accredible References API
  slug: accredible-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-references-api-openapi.yml
- filename: accredible-sso-api-openapi.yml
  format: yaml
  label: Accredible SSO API
  slug: accredible-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-sso-api-openapi.yml
- filename: accredible-team-members-api-openapi.yml
  format: yaml
  label: Accredible Team Members API
  slug: accredible-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/openapi/accredible-team-members-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: accredible.com
  spf: true
hosts:
- cert_expires: Oct  8 11:14:37 2026 GMT
  host: www.accredible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:24:37 2026 GMT
  host: docs.api.accredible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.accredible.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accredible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accredible, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Accredible
provider_slug: accredible
slug: accredible-domain-security
source_filename: accredible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accredible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:14:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.accredible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:24:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.accredible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: accredible.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredible/refs/heads/main/security/accredible-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Credentials
- Certificates
- Badges
- Open Badges
- Credentialing
- Verification
- Digital Badges
---
