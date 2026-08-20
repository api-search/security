---
api_specs:
- filename: cybelangel-platform-reports-openapi.yml
  format: yaml
  label: CybelAngel Reports API
  slug: cybelangel-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-platform-reports-openapi.yml
- filename: cybelangel-alerts-openapi.yml
  format: yaml
  label: CybelAngel Alerts API
  slug: cybelangel-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-alerts-openapi.yml
- filename: cybelangel-adm-inventory-openapi.yml
  format: yaml
  label: CybelAngel ADM Inventory API
  slug: cybelangel-adm-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-adm-inventory-openapi.yml
- filename: cybelangel-keywords-openapi.yml
  format: yaml
  label: CybelAngel Keywords API
  slug: cybelangel-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-keywords-openapi.yml
- filename: cybelangel-threat-intelligence-openapi.yml
  format: yaml
  label: CybelAngel Threat Intelligence API
  slug: cybelangel-threat-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-threat-intelligence-openapi.yml
- filename: cybelangel-audit-logs-openapi.yml
  format: yaml
  label: CybelAngel Audit Logs API
  slug: cybelangel-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-audit-logs-openapi.yml
- filename: cybelangel-partner-openapi.yml
  format: yaml
  label: CybelAngel Partner API
  slug: cybelangel-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/openapi/cybelangel-partner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cybelangel.com
  spf: true
hosts:
- cert_expires: Nov 14 12:28:35 2026 GMT
  host: www.cybelangel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 13:15:50 2026 GMT
  host: developers.cybelangel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:29:26 2026 GMT
  host: platform.cybelangel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:29:26 2026 GMT
  host: api.cybelangel.com
  hsts: false
  hsts_max_age: null
  https: true
  note: The API host for six of the seven published APIs. Added by hand — the probe script caps itself at three hosts. Root returns HTTP/2 404 text/plain "404 page not found" with x-content-type-options nosniff and NO Strict-Transport-Security header, so this host is the one gap in an otherwise HSTS-everywhere estate.
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:56:59 2026 GMT
  host: auth.cybelangel.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 tenant that mints every bearer token; serves OIDC discovery and JWKS. Added by hand for the same reason as api.cybelangel.com.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cybelangel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CybelAngel, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CybelAngel
provider_slug: cybelangel
slug: cybelangel-domain-security
source_filename: cybelangel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybelangel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 12:28:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cybelangel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.cybelangel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:29:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cybelangel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:29:26 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    The API host for six of the seven published APIs. Added by hand — the probe script\n    caps itself at three hosts. Root returns HTTP/2 404 text/plain \"404 page not found\"\n    with x-content-type-options nosniff and NO Strict-Transport-Security header,\
  \ so this\n    host is the one gap in an otherwise HSTS-everywhere estate.\n- host: auth.cybelangel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:56:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Auth0 tenant that mints every bearer token; serves OIDC discovery and JWKS.\n    Added by hand for the same reason as api.cybelangel.com.\ndomains:\n- domain: cybelangel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybelangel/refs/heads/main/security/cybelangel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- external-attack-surface-management
- data-breach-prevention
- Credential Intelligence
- Brand Protection
- Dark Web Monitoring
- Digital Risk Protection
- STIX
- security-alerts
- Asset Inventory
- Audit Logs
---
