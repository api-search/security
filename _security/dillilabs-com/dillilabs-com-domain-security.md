---
api_specs:
- filename: dillilabs-com-analyze-api-openapi.yml
  format: yaml
  label: Dilli Labs Analyze API
  slug: dillilabs-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-analyze-api-openapi.yml
- filename: dillilabs-com-health-api-openapi.yml
  format: yaml
  label: Dilli Labs Health API
  slug: dillilabs-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-health-api-openapi.yml
- filename: dillilabs-com-privacy-api-openapi.yml
  format: yaml
  label: Dilli Labs Privacy API
  slug: dillilabs-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-privacy-api-openapi.yml
- filename: dillilabs-com-purchase-api-openapi.yml
  format: yaml
  label: Dilli Labs Purchase API
  slug: dillilabs-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-purchase-api-openapi.yml
- filename: dillilabs-com-user-api-openapi.yml
  format: yaml
  label: Dilli Labs User API
  slug: dillilabs-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dillilabs.com
  spf: true
hosts:
- cert_expires: Dec  7 21:24:27 2026 GMT
  host: www.dillilabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 05:32:23 2026 GMT
  host: deva.dillilabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dilli Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dilli Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dilli Labs
provider_slug: dillilabs-com
slug: dillilabs-com-domain-security
source_filename: dillilabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dillilabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 21:24:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: deva.dillilabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 05:32:23 2026 GMT\n  hsts: false\ndomains:\n- domain: dillilabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dillilabs-com/security/dillilabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Verification
- IP Geolocation
- IP Validation
- Profanity Detection
- MCP
- Software-as-a-Service
- Web Hosting
- Software Development
---
