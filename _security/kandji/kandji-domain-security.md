---
api_specs:
- filename: kandji-audit-api-openapi.yml
  format: yaml
  label: Iru Audit API
  slug: kandji-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-audit-api-openapi.yml
- filename: kandji-behavioral-detections-api-openapi.yml
  format: yaml
  label: Iru Behavioral Detections API
  slug: kandji-behavioral-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-behavioral-detections-api-openapi.yml
- filename: kandji-blueprints-api-openapi.yml
  format: yaml
  label: Iru Blueprints API
  slug: kandji-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-blueprints-api-openapi.yml
- filename: kandji-devices-api-openapi.yml
  format: yaml
  label: Iru Devices API
  slug: kandji-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-devices-api-openapi.yml
- filename: kandji-integrations-api-openapi.yml
  format: yaml
  label: Iru Integrations API
  slug: kandji-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-integrations-api-openapi.yml
- filename: kandji-library-api-openapi.yml
  format: yaml
  label: Iru Library API
  slug: kandji-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-library-api-openapi.yml
- filename: kandji-prism-api-openapi.yml
  format: yaml
  label: Iru Prism API
  slug: kandji-prism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-prism-api-openapi.yml
- filename: kandji-self-service-api-openapi.yml
  format: yaml
  label: Iru Self Service API
  slug: kandji-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-self-service-api-openapi.yml
- filename: kandji-settings-api-openapi.yml
  format: yaml
  label: Iru Settings API
  slug: kandji-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-settings-api-openapi.yml
- filename: kandji-tags-api-openapi.yml
  format: yaml
  label: Iru Tags API
  slug: kandji-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-tags-api-openapi.yml
- filename: kandji-threat-details-api-openapi.yml
  format: yaml
  label: Iru Threat Details API
  slug: kandji-threat-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-threat-details-api-openapi.yml
- filename: kandji-upload-to-s3-api-openapi.yml
  format: yaml
  label: Iru Upload To S3 API
  slug: kandji-upload-to-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-upload-to-s3-api-openapi.yml
- filename: kandji-users-api-openapi.yml
  format: yaml
  label: Iru Users API
  slug: kandji-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-users-api-openapi.yml
- filename: kandji-vulnerability-management-api-openapi.yml
  format: yaml
  label: Iru Vulnerability Management API
  slug: kandji-vulnerability-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-vulnerability-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: iru.com
  spf: true
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kandji.io
  spf: true
hosts:
- cert_expires: Oct  2 22:10:20 2026 GMT
  host: www.iru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:58:16 2026 GMT
  host: api-docs.kandji.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 21:02:52 2026 GMT
  host: your-subdomain.api.kandji.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kandji Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iru, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Iru
provider_slug: kandji
slug: kandji-domain-security
source_filename: kandji-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:10:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.kandji.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-subdomain.api.kandji.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iru.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kandji.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/security/kandji-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Device Management
- Mobile Device Management
- apple-management
- Endpoint Security
- endpoint-detection-response
- Vulnerability Management
- Compliance Automation
- Workforce Identity
- IT Operations
- MCP
- agent-native
---
