---
api_specs:
- filename: usace-cwms-data-api-openapi.yml
  format: yaml
  label: USACE Corps Water Management System Data API
  slug: cwms-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-department-of-defense/refs/heads/main/openapi/usace-cwms-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: army.mil
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: defense.gov
  spf: true
hosts:
- cert_expires: Sep 30 16:46:59 2026 GMT
  host: cwms-data.usace.army.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: corpslocks.usace.army.mil
  https: false
- cert_expires: Jul 29 18:07:45 2026 GMT
  host: data.defense.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Department Of Defense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Department of Defense, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Department of Defense
provider_slug: us-department-of-defense
slug: us-department-of-defense-domain-security
source_filename: us-department-of-defense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cwms-data.usace.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:46:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: corpslocks.usace.army.mil\n  https: false\n- host: data.defense.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 18:07:45 2026 GMT\n  hsts: null\ndomains:\n- domain: army.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: defense.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-department-of-defense/refs/heads/main/security/us-department-of-defense-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Defense
- Military
- Water Management
- Waterways
- Open Data
---
