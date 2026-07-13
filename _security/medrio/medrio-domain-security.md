---
api_specs:
- filename: swagger.json
  format: json
  label: Medrio Studies API
  slug: medrio-studies-api
  spec_type: OpenAPI
  url: https://connectapi.medrio.com/swagger/v1/swagger.json
- filename: swagger.json
  format: json
  label: Medrio Subjects API
  slug: medrio-subjects-api
  spec_type: OpenAPI
  url: https://connectapi.medrio.com/swagger/v1/swagger.json
- filename: swagger.json
  format: json
  label: Medrio Data Entry API
  slug: medrio-data-entry-api
  spec_type: OpenAPI
  url: https://connectapi.medrio.com/swagger/v1/swagger.json
- filename: swagger.json
  format: json
  label: Medrio Users and Memberships API
  slug: medrio-users-memberships-api
  spec_type: OpenAPI
  url: https://connectapi.medrio.com/swagger/v1/swagger.json
- filename: swagger.json
  format: json
  label: Medrio Subscriptions API
  slug: medrio-subscriptions-api
  spec_type: OpenAPI
  url: https://connectapi.medrio.com/swagger/v1/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medrio.com
  spf: true
hosts:
- cert_expires: Sep 23 17:22:45 2026 GMT
  host: medrio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: connectapi.medrio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: esource.medrio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medrio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medrio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medrio
provider_slug: medrio
slug: medrio-domain-security
source_filename: medrio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medrio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:22:45 2026 GMT\n  hsts: false\n- host: connectapi.medrio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: null\n- host: esource.medrio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: medrio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medrio/refs/heads/main/security/medrio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- eClinical
- ePRO
- eCOA
- Clinical Data
- Life Sciences
- Healthcare
---
