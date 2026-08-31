---
api_specs:
- filename: galatea-bio-auth-api-openapi.yml
  format: yaml
  label: Galatea Bio Auth API
  slug: galatea-bio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-auth-api-openapi.yml
- filename: galatea-bio-credit-api-openapi.yml
  format: yaml
  label: Galatea Bio Credit API
  slug: galatea-bio-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-credit-api-openapi.yml
- filename: galatea-bio-dashboard-api-openapi.yml
  format: yaml
  label: Galatea Bio Dashboard API
  slug: galatea-bio-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-dashboard-api-openapi.yml
- filename: galatea-bio-data-api-openapi.yml
  format: yaml
  label: Galatea Bio Data API
  slug: galatea-bio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-data-api-openapi.yml
- filename: galatea-bio-exec-api-openapi.yml
  format: yaml
  label: Galatea Bio Exec API
  slug: galatea-bio-exec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-exec-api-openapi.yml
- filename: galatea-bio-internal-api-openapi.yml
  format: yaml
  label: Galatea Bio Internal API
  slug: galatea-bio-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-internal-api-openapi.yml
- filename: galatea-bio-notification-api-openapi.yml
  format: yaml
  label: Galatea Bio Notification API
  slug: galatea-bio-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-notification-api-openapi.yml
- filename: galatea-bio-organizations-api-openapi.yml
  format: yaml
  label: Galatea Bio Organizations API
  slug: galatea-bio-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-organizations-api-openapi.yml
- filename: galatea-bio-statistics-api-openapi.yml
  format: yaml
  label: Galatea Bio Statistics API
  slug: galatea-bio-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-statistics-api-openapi.yml
- filename: galatea-bio-users-api-openapi.yml
  format: yaml
  label: Galatea Bio Users API
  slug: galatea-bio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: galatea.bio
  spf: true
hosts:
- cert_expires: Nov 10 10:11:25 2026 GMT
  host: galatea.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:55:40 2026 GMT
  host: docs.galatea.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 11:00:23 2026 GMT
  host: api.galatea.bio
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galatea Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galatea Bio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Galatea Bio
provider_slug: galatea-bio
slug: galatea-bio-domain-security
source_filename: galatea-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:11:25 2026 GMT\n  hsts: false\n- host: docs.galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:55:40 2026 GMT\n  hsts: false\n- host: api.galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 11:00:23 2026 GMT\n  hsts: null\ndomains:\n- domain: galatea.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/security/galatea-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- genomics
- bioinformatics
- ancestry
- precision-medicine
- polygenic-risk-score
- clinical-laboratory
- genetic-testing
- biobank
- life-sciences
- Health
- sequencing
---
