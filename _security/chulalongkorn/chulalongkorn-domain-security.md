---
api_specs:
- filename: chulalongkorn-curriculum-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Curriculum API
  slug: chulalongkorn-curriculum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-curriculum-api-openapi.yml
- filename: chulalongkorn-meta-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Meta API
  slug: chulalongkorn-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-meta-api-openapi.yml
- filename: chulalongkorn-about-api-openapi.yml
  format: yaml
  label: Chulalongkorn University About API
  slug: chulalongkorn-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-about-api-openapi.yml
- filename: chulalongkorn-admin-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Admin API
  slug: chulalongkorn-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-admin-api-openapi.yml
- filename: chulalongkorn-chulasso-service-api-openapi.yml
  format: yaml
  label: Chulalongkorn University ChulaSSO Service API
  slug: chulalongkorn-chulasso-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-chulasso-service-api-openapi.yml
- filename: chulalongkorn-html-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Html API
  slug: chulalongkorn-html-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-html-api-openapi.yml
- filename: chulalongkorn-login-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Login API
  slug: chulalongkorn-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-login-api-openapi.yml
- filename: chulalongkorn-logout-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Logout API
  slug: chulalongkorn-logout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-logout-api-openapi.yml
- filename: chulalongkorn-myapps-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Myapps API
  slug: chulalongkorn-myapps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-myapps-api-openapi.yml
- filename: chulalongkorn-qr-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Qr API
  slug: chulalongkorn-qr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-qr-api-openapi.yml
- filename: chulalongkorn-qrvalidation-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Qr Validation API
  slug: chulalongkorn-qrvalidation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-qrvalidation-api-openapi.yml
- filename: chulalongkorn-servicevalidation-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Service Validation API
  slug: chulalongkorn-servicevalidation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-servicevalidation-api-openapi.yml
- filename: chulalongkorn-tickets-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Tickets API
  slug: chulalongkorn-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-tickets-api-openapi.yml
- filename: chulalongkorn-users-api-openapi.yml
  format: yaml
  label: Chulalongkorn University Users API
  slug: chulalongkorn-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-users-api-openapi.yml
- filename: chulalongkorn-2-fa-api-openapi.yml
  format: yaml
  label: Chulalongkorn University 2 FA API
  slug: chulalongkorn-2-fa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chulalongkorn/openapi/chulalongkorn-2-fa-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chula.ac.th
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.chula.ac.th
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 00:56:49 2026 GMT
  host: account.it.chula.ac.th
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 06:14:28 2026 GMT
  host: digiverse.chula.ac.th
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chulalongkorn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chulalongkorn University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chulalongkorn University
provider_slug: chulalongkorn
slug: chulalongkorn-domain-security
source_filename: chulalongkorn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chula.ac.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: account.it.chula.ac.th\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 00:56:49 2026 GMT\n  hsts: null\n- host: digiverse.chula.ac.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:14:28 2026 GMT\n  hsts: false\ndomains:\n- domain: chula.ac.th\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chulalongkorn/security/chulalongkorn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Thailand
- Bangkok
- Identity Federation
- SSO
- Course Catalog
- Research Repository
- Library
- Open Access
- OAI-PMH
---
