---
api_specs:
- filename: domaindrift-io-alerts-api-openapi.yml
  format: yaml
  label: DomainDrift Alerts API
  slug: domaindrift-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-alerts-api-openapi.yml
- filename: domaindrift-io-changes-api-openapi.yml
  format: yaml
  label: DomainDrift Changes API
  slug: domaindrift-io-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-changes-api-openapi.yml
- filename: domaindrift-io-domains-api-openapi.yml
  format: yaml
  label: DomainDrift Domains API
  slug: domaindrift-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-domains-api-openapi.yml
- filename: domaindrift-io-health-api-openapi.yml
  format: yaml
  label: DomainDrift Health API
  slug: domaindrift-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-health-api-openapi.yml
- filename: domaindrift-io-scan-api-openapi.yml
  format: yaml
  label: DomainDrift Scan API
  slug: domaindrift-io-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-scan-api-openapi.yml
- filename: domaindrift-io-stream-api-openapi.yml
  format: yaml
  label: DomainDrift Stream API
  slug: domaindrift-io-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaindrift-io/openapi/domaindrift-io-stream-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: domaindrift.io
  spf: true
hosts:
- cert_expires: Jan  3 21:35:16 2027 GMT
  host: domaindrift.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domaindrift Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainDrift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DomainDrift
provider_slug: domaindrift-io
slug: domaindrift-io-domain-security
source_filename: domaindrift-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domaindrift.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:35:16 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: domaindrift.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/domaindrift-io/security/domaindrift-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Monitoring
- Domain
- Telemetry
---
