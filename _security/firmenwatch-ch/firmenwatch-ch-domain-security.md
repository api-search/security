---
api_specs:
- filename: firmenwatch-ch-aktionen-api-openapi.yml
  format: yaml
  label: Firmenwatch Aktionen API
  slug: firmenwatch-ch-aktionen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-aktionen-api-openapi.yml
- filename: firmenwatch-ch-betrieb-api-openapi.yml
  format: yaml
  label: Firmenwatch Betrieb API
  slug: firmenwatch-ch-betrieb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-betrieb-api-openapi.yml
- filename: firmenwatch-ch-ereignisse-api-openapi.yml
  format: yaml
  label: Firmenwatch Ereignisse API
  slug: firmenwatch-ch-ereignisse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-ereignisse-api-openapi.yml
- filename: firmenwatch-ch-firmen-api-openapi.yml
  format: yaml
  label: Firmenwatch Firmen API
  slug: firmenwatch-ch-firmen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-firmen-api-openapi.yml
- filename: firmenwatch-ch-identitaet-api-openapi.yml
  format: yaml
  label: Firmenwatch Identitaet API
  slug: firmenwatch-ch-identitaet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-identitaet-api-openapi.yml
- filename: firmenwatch-ch-portfolios-api-openapi.yml
  format: yaml
  label: Firmenwatch Portfolios API
  slug: firmenwatch-ch-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-portfolios-api-openapi.yml
- filename: firmenwatch-ch-uid-api-openapi.yml
  format: yaml
  label: Firmenwatch UID API
  slug: firmenwatch-ch-uid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmenwatch-ch/openapi/firmenwatch-ch-uid-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firmenwatch.ch
  spf: true
hosts:
- cert_expires: Jan 25 07:21:54 2027 GMT
  host: firmenwatch.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmenwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firmenwatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Firmenwatch
provider_slug: firmenwatch-ch
slug: firmenwatch-ch-domain-security
source_filename: firmenwatch-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmenwatch.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 07:21:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: firmenwatch.ch\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/firmenwatch-ch/security/firmenwatch-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Swiss
- Monitoring
- Commercial-Register
- Alerts
- Business Intelligence
---
