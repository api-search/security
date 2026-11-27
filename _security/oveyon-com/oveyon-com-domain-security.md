---
api_specs:
- filename: oveyon-com-allow-block-lists-api-openapi.yml
  format: yaml
  label: Oveyon Allow/Block lists API
  slug: oveyon-com-allow-block-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-allow-block-lists-api-openapi.yml
- filename: oveyon-com-domains-api-openapi.yml
  format: yaml
  label: Oveyon Domains API
  slug: oveyon-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-domains-api-openapi.yml
- filename: oveyon-com-inbound-api-openapi.yml
  format: yaml
  label: Oveyon Inbound API
  slug: oveyon-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-inbound-api-openapi.yml
- filename: oveyon-com-ip-rules-api-openapi.yml
  format: yaml
  label: Oveyon IP rules API
  slug: oveyon-com-ip-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-ip-rules-api-openapi.yml
- filename: oveyon-com-logs-api-openapi.yml
  format: yaml
  label: Oveyon Logs API
  slug: oveyon-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-logs-api-openapi.yml
- filename: oveyon-com-marketing-experimental-api-openapi.yml
  format: yaml
  label: Oveyon Marketing (experimental) API
  slug: oveyon-com-marketing-experimental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-marketing-experimental-api-openapi.yml
- filename: oveyon-com-messages-api-openapi.yml
  format: yaml
  label: Oveyon Messages API
  slug: oveyon-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-messages-api-openapi.yml
- filename: oveyon-com-meta-api-openapi.yml
  format: yaml
  label: Oveyon Meta API
  slug: oveyon-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-meta-api-openapi.yml
- filename: oveyon-com-nps-csat-surveys-api-openapi.yml
  format: yaml
  label: Oveyon NPS/CSAT surveys API
  slug: oveyon-com-nps-csat-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-nps-csat-surveys-api-openapi.yml
- filename: oveyon-com-send-policies-api-openapi.yml
  format: yaml
  label: Oveyon Send policies API
  slug: oveyon-com-send-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-send-policies-api-openapi.yml
- filename: oveyon-com-sending-api-openapi.yml
  format: yaml
  label: Oveyon Sending API
  slug: oveyon-com-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-sending-api-openapi.yml
- filename: oveyon-com-suppressions-api-openapi.yml
  format: yaml
  label: Oveyon Suppressions API
  slug: oveyon-com-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-suppressions-api-openapi.yml
- filename: oveyon-com-templates-api-openapi.yml
  format: yaml
  label: Oveyon Templates API
  slug: oveyon-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-templates-api-openapi.yml
- filename: oveyon-com-utilities-api-openapi.yml
  format: yaml
  label: Oveyon Utilities API
  slug: oveyon-com-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-utilities-api-openapi.yml
- filename: oveyon-com-webhooks-api-openapi.yml
  format: yaml
  label: Oveyon Webhooks API
  slug: oveyon-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oveyon-com/openapi/oveyon-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: oveyon.com
  spf: true
hosts:
- cert_expires: Jan  9 02:17:09 2027 GMT
  host: oveyon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oveyon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oveyon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Oveyon
provider_slug: oveyon-com
slug: oveyon-com-domain-security
source_filename: oveyon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oveyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 02:17:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oveyon.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/oveyon-com/security/oveyon-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transactional Email
- Email API
- SMTP
- Deliverability
- Audit Trail
- Webhook
- Fintech
- Healthcare
---
