---
api_specs:
- filename: ukm-content-api-openapi.yml
  format: yaml
  label: Universiti Kebangsaan Malaysia Content API
  slug: ukm-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-content-api-openapi.yml
- filename: ukm-discovery-api-openapi.yml
  format: yaml
  label: Universiti Kebangsaan Malaysia Discovery API
  slug: ukm-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-discovery-api-openapi.yml
- filename: ukm-metadata-api-openapi.yml
  format: yaml
  label: Universiti Kebangsaan Malaysia Metadata API
  slug: ukm-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-metadata-api-openapi.yml
- filename: ukm-oai-pmh-api-openapi.yml
  format: yaml
  label: Universiti Kebangsaan Malaysia OAI PMH API
  slug: ukm-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-oai-pmh-api-openapi.yml
- filename: ukm-single-sign-on-api-openapi.yml
  format: yaml
  label: Universiti Kebangsaan Malaysia Single Sign-On API
  slug: ukm-single-sign-on-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/openapi/ukm-single-sign-on-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ukm.my
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.ukm.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ptsldigital.ukm.my
  https: false
- host: journalarticle.ukm.my
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ukm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Kebangsaan Malaysia, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Universiti Kebangsaan Malaysia
provider_slug: ukm
slug: ukm-domain-security
source_filename: ukm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ukm.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ptsldigital.ukm.my\n  https: false\n- host: journalarticle.ukm.my\n  https: false\ndomains:\n- domain: ukm.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukm/refs/heads/main/security/ukm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Research
- Malaysia
- Southeast Asia
- Identity Federation
- SAML
- Research Repository
- Institutional Repository
- OAI-PMH
- Open Access
- Scholarly Publishing
- Library
- Theses
---
