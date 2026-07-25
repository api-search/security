---
api_specs:
- filename: epfl-categories-api-openapi.yml
  format: yaml
  label: EPFL Categories API
  slug: epfl-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-categories-api-openapi.yml
- filename: epfl-channels-api-openapi.yml
  format: yaml
  label: EPFL Channels API
  slug: epfl-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-channels-api-openapi.yml
- filename: epfl-domains-api-openapi.yml
  format: yaml
  label: EPFL Domains API
  slug: epfl-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-domains-api-openapi.yml
- filename: epfl-events-api-openapi.yml
  format: yaml
  label: EPFL Events API
  slug: epfl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-events-api-openapi.yml
- filename: epfl-faculties-api-openapi.yml
  format: yaml
  label: EPFL Faculties API
  slug: epfl-faculties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-faculties-api-openapi.yml
- filename: epfl-mementos-api-openapi.yml
  format: yaml
  label: EPFL Mementos API
  slug: epfl-mementos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-mementos-api-openapi.yml
- filename: epfl-news-api-openapi.yml
  format: yaml
  label: EPFL News API
  slug: epfl-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-news-api-openapi.yml
- filename: epfl-projects-api-openapi.yml
  format: yaml
  label: EPFL Projects API
  slug: epfl-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-projects-api-openapi.yml
- filename: epfl-publics-api-openapi.yml
  format: yaml
  label: EPFL Publics API
  slug: epfl-publics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-publics-api-openapi.yml
- filename: epfl-registrations-api-openapi.yml
  format: yaml
  label: EPFL Registrations API
  slug: epfl-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-registrations-api-openapi.yml
- filename: epfl-spoken-languages-api-openapi.yml
  format: yaml
  label: EPFL Spoken Languages API
  slug: epfl-spoken-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-spoken-languages-api-openapi.yml
- filename: epfl-themes-api-openapi.yml
  format: yaml
  label: EPFL Themes API
  slug: epfl-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-themes-api-openapi.yml
- filename: epfl-vulgarizations-api-openapi.yml
  format: yaml
  label: EPFL Vulgarizations API
  slug: epfl-vulgarizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-vulgarizations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epfl.ch
  spf: true
hosts:
- cert_expires: Aug 14 12:58:47 2026 GMT
  host: www.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 23:32:22 2026 GMT
  host: actu.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:41:00 2026 GMT
  host: memento.epfl.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epfl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPFL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EPFL
provider_slug: epfl
slug: epfl-domain-security
source_filename: epfl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 12:58:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: actu.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: memento.epfl.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:41:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epfl.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/security/epfl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Switzerland
- Europe
---
