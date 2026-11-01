---
api_specs:
- filename: lastscanned-com-account-api-openapi.yml
  format: yaml
  label: lastscanned Account API
  slug: lastscanned-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-account-api-openapi.yml
- filename: lastscanned-com-carriers-api-openapi.yml
  format: yaml
  label: lastscanned Carriers API
  slug: lastscanned-com-carriers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-carriers-api-openapi.yml
- filename: lastscanned-com-track-api-openapi.yml
  format: yaml
  label: lastscanned Track API
  slug: lastscanned-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-track-api-openapi.yml
- filename: lastscanned-com-tracking-api-openapi.yml
  format: yaml
  label: lastscanned Tracking API
  slug: lastscanned-com-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-tracking-api-openapi.yml
- filename: lastscanned-com-watches-api-openapi.yml
  format: yaml
  label: lastscanned Watches API
  slug: lastscanned-com-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-watches-api-openapi.yml
- filename: lastscanned-com-webhooks-api-openapi.yml
  format: yaml
  label: lastscanned Webhooks API
  slug: lastscanned-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lastscanned.com
  spf: true
hosts:
- cert_expires: Jan 24 23:12:31 2027 GMT
  host: lastscanned.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lastscanned Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lastscanned, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: lastscanned
provider_slug: lastscanned-com
slug: lastscanned-com-domain-security
source_filename: lastscanned-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lastscanned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:12:31 2027 GMT\n  hsts: false\ndomains:\n- domain: lastscanned.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lastscanned-com/security/lastscanned-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Tracking
- Logistics
- API
- MCP
---
