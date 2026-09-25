---
api_specs:
- filename: lifemine-board-api-openapi.yml
  format: yaml
  label: LifeMine Board API
  slug: lifemine-board-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-board-api-openapi.yml
- filename: lifemine-departments-api-openapi.yml
  format: yaml
  label: LifeMine Departments API
  slug: lifemine-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-departments-api-openapi.yml
- filename: lifemine-education-api-openapi.yml
  format: yaml
  label: LifeMine Education API
  slug: lifemine-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-education-api-openapi.yml
- filename: lifemine-jobs-api-openapi.yml
  format: yaml
  label: LifeMine Jobs API
  slug: lifemine-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-jobs-api-openapi.yml
- filename: lifemine-offices-api-openapi.yml
  format: yaml
  label: LifeMine Offices API
  slug: lifemine-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-offices-api-openapi.yml
- filename: lifemine-sections-api-openapi.yml
  format: yaml
  label: LifeMine Sections API
  slug: lifemine-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/openapi/lifemine-sections-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dnssec: false
  domain: lifeminetx.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:17:19 2026 GMT
  host: lifeminetx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Lifemine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LifeMine, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LifeMine
provider_slug: lifemine
slug: lifemine-domain-security
source_filename: lifemine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: lifeminetx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:17:19 2026 GMT\n  hsts: false\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lifeminetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifemine/refs/heads/main/security/lifemine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Clinical Trials
- Genomics
- Content
- Careers
- WordPress
---
