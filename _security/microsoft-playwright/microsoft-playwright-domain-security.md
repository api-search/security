---
api_specs:
- filename: microsoft-playwright-accountquotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Account Quotas API
  slug: microsoft-playwright-accountquotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accountquotas-api-openapi.yml
- filename: microsoft-playwright-operations-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Operations API
  slug: microsoft-playwright-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-operations-api-openapi.yml
- filename: microsoft-playwright-quotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Quotas API
  slug: microsoft-playwright-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-quotas-api-openapi.yml
- filename: microsoft-playwright-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Accounts API
  slug: microsoft-playwright-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accounts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playwright.dev
  spf: false
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 19 00:41:51 2027 GMT
  host: playwright.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 09:41:22 2027 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Microsoft Playwright Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Playwright, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Microsoft Playwright
provider_slug: microsoft-playwright
slug: microsoft-playwright-domain-security
source_filename: microsoft-playwright-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playwright.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 00:41:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:41:22 2027 GMT\n  hsts: null\ndomains:\n- domain: playwright.dev\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-playwright/security/microsoft-playwright-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Automation
- End-to-End Testing
- Microsoft
- Testing
- Open Source
- MCP
- Microsoft Azure
---
