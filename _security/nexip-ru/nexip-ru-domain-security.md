---
api_specs:
- filename: nexip-ru-billing-api-openapi.yml
  format: yaml
  label: NexIP Billing API
  slug: nexip-ru-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-billing-api-openapi.yml
- filename: nexip-ru-comparisons-api-openapi.yml
  format: yaml
  label: NexIP Comparisons API
  slug: nexip-ru-comparisons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-comparisons-api-openapi.yml
- filename: nexip-ru-monitoring-api-openapi.yml
  format: yaml
  label: NexIP Monitoring API
  slug: nexip-ru-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-monitoring-api-openapi.yml
- filename: nexip-ru-notifications-api-openapi.yml
  format: yaml
  label: NexIP Notifications API
  slug: nexip-ru-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-notifications-api-openapi.yml
- filename: nexip-ru-public-entities-api-openapi.yml
  format: yaml
  label: NexIP Public Entities API
  slug: nexip-ru-public-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-public-entities-api-openapi.yml
- filename: nexip-ru-reports-api-openapi.yml
  format: yaml
  label: NexIP Reports API
  slug: nexip-ru-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-reports-api-openapi.yml
- filename: nexip-ru-seo-audit-api-openapi.yml
  format: yaml
  label: NexIP SEO Audit API
  slug: nexip-ru-seo-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-seo-audit-api-openapi.yml
- filename: nexip-ru-system-api-openapi.yml
  format: yaml
  label: NexIP System API
  slug: nexip-ru-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-system-api-openapi.yml
- filename: nexip-ru-tools-api-openapi.yml
  format: yaml
  label: NexIP Tools API
  slug: nexip-ru-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-tools-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexip.ru
  spf: true
hosts:
- cert_expires: Dec 22 10:23:14 2026 GMT
  host: nexip.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NexIP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NexIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NexIP
provider_slug: nexip-ru
slug: nexip-ru-domain-security
source_filename: nexip-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexip.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 10:23:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexip.ru\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nexip-ru/security/nexip-ru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
