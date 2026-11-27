---
api_specs:
- filename: taktovka-com-absences-api-openapi.yml
  format: yaml
  label: Taktovka Absences API
  slug: taktovka-com-absences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-absences-api-openapi.yml
- filename: taktovka-com-attendance-api-openapi.yml
  format: yaml
  label: Taktovka Attendance API
  slug: taktovka-com-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-attendance-api-openapi.yml
- filename: taktovka-com-company-api-openapi.yml
  format: yaml
  label: Taktovka Company API
  slug: taktovka-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-company-api-openapi.yml
- filename: taktovka-com-meta-api-openapi.yml
  format: yaml
  label: Taktovka Meta API
  slug: taktovka-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-meta-api-openapi.yml
- filename: taktovka-com-people-api-openapi.yml
  format: yaml
  label: Taktovka People API
  slug: taktovka-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-people-api-openapi.yml
- filename: taktovka-com-schedules-api-openapi.yml
  format: yaml
  label: Taktovka Schedules API
  slug: taktovka-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taktovka-com/openapi/taktovka-com-schedules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: taktovka.com
  spf: true
hosts:
- cert_expires: Feb  8 23:48:49 2027 GMT
  host: taktovka.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taktovka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taktovka, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Taktovka
provider_slug: taktovka-com
slug: taktovka-com-domain-security
source_filename: taktovka-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taktovka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:48:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taktovka.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/taktovka-com/security/taktovka-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
