---
api_specs:
- filename: sensedia-openapi-generated.yml
  format: yaml
  label: Sensedia API
  slug: sensedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_ae-authored/sensedia-openapi-generated.yml
- filename: sensedia-old-openapi.yml
  format: yaml
  label: Sensedia Old API
  slug: sensedia-old-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-old-openapi.yml
- filename: sensedia-current-openapi.yml
  format: yaml
  label: Sensedia Current API
  slug: sensedia-current-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-current-openapi.yml
- filename: sensedia-teste-openapi.yml
  format: yaml
  label: Sensedia Teste API
  slug: sensedia-teste-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-teste-openapi.yml
- filename: sensedia-old-openapi.yml
  format: yaml
  label: Sensedia Old API
  slug: sensedia-old-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-old-openapi.yml
- filename: sensedia-current-openapi.yml
  format: yaml
  label: Sensedia Current API
  slug: sensedia-current-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-current-openapi.yml
- filename: sensedia-teste-openapi.yml
  format: yaml
  label: Sensedia Teste API
  slug: sensedia-teste-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/openapi/_original/sensedia-teste-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sensedia.com
  spf: true
hosts:
- cert_expires: Dec  5 10:03:38 2026 GMT
  host: www.sensedia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sensedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sensedia
provider_slug: sensedia
slug: sensedia-domain-security
source_filename: sensedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sensedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 10:03:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sensedia.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensedia/refs/heads/main/security/sensedia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Management
- Integration
- Enterprise
- AI
---
