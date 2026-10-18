---
api_specs:
- filename: laserfiche-oauth-api-openapi.yml
  format: yaml
  label: Laserfiche OAuth API
  slug: laserfiche-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-oauth-api-openapi.yml
- filename: laserfiche-odata4-api-openapi.yml
  format: yaml
  label: Laserfiche Odata4 API
  slug: laserfiche-odata4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-odata4-api-openapi.yml
- filename: laserfiche-repositories-api-openapi.yml
  format: yaml
  label: Laserfiche Repositories API
  slug: laserfiche-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-repositories-api-openapi.yml
- filename: laserfiche-repository-api-openapi.yml
  format: yaml
  label: Laserfiche Repository API
  slug: laserfiche-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/laserfiche-repository-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: laserfiche.com
  spf: true
hosts:
- cert_expires: Dec 30 06:15:35 2026 GMT
  host: www.laserfiche.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laserfiche Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laserfiche, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Laserfiche
provider_slug: laserfiche
slug: laserfiche-domain-security
source_filename: laserfiche-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laserfiche.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 06:15:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: laserfiche.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/security/laserfiche-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EnterpriseContentManagement
- Document Management
- ProcessAutomation
- Artificial Intelligence
---
