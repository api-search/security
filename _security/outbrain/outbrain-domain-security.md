---
api_specs:
- filename: outbrain-authentication-api-openapi.yml
  format: yaml
  label: Outbrain Authentication API
  slug: outbrain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-authentication-api-openapi.yml
- filename: outbrain-budgets-api-openapi.yml
  format: yaml
  label: Outbrain Budgets API
  slug: outbrain-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-budgets-api-openapi.yml
- filename: outbrain-campaigns-api-openapi.yml
  format: yaml
  label: Outbrain Campaigns API
  slug: outbrain-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-campaigns-api-openapi.yml
- filename: outbrain-conversions-api-openapi.yml
  format: yaml
  label: Outbrain Conversions API
  slug: outbrain-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-conversions-api-openapi.yml
- filename: outbrain-events-api-openapi.yml
  format: yaml
  label: Outbrain Events API
  slug: outbrain-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-events-api-openapi.yml
- filename: outbrain-marketers-api-openapi.yml
  format: yaml
  label: Outbrain Marketers API
  slug: outbrain-marketers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-marketers-api-openapi.yml
- filename: outbrain-promotedlinks-api-openapi.yml
  format: yaml
  label: Outbrain PromotedLinks API
  slug: outbrain-promotedlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-promotedlinks-api-openapi.yml
- filename: outbrain-recommendations-api-openapi.yml
  format: yaml
  label: Outbrain Recommendations API
  slug: outbrain-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-recommendations-api-openapi.yml
- filename: outbrain-reporting-api-openapi.yml
  format: yaml
  label: Outbrain Reporting API
  slug: outbrain-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-reporting-api-openapi.yml
- filename: outbrain-targeting-api-openapi.yml
  format: yaml
  label: Outbrain Targeting API
  slug: outbrain-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-targeting-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "email:caa@teads.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: outbrain.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@teads.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teads.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.outbrain.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:16:14 2026 GMT
  host: www.teads.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:25:26 2026 GMT
  host: developer.outbrain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outbrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outbrain, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Outbrain
provider_slug: outbrain
slug: outbrain-domain-security
source_filename: outbrain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.outbrain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: www.teads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:16:14 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.outbrain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:25:26 2026 GMT\n  hsts: false\ndomains:\n- domain: outbrain.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"email:caa@teads.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: teads.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@teads.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue\
  \ \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/security/outbrain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Native Advertising
- Open Web
- CTV
- Connected TV
- Video Advertising
- Content Discovery
- Programmatic
- Performance Marketing
- AdTech
- Teads
---
