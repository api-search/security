---
api_specs:
- filename: hmm21-arrival-notice-api-openapi.yml
  format: yaml
  label: HMM Arrival Notice API
  slug: hmm21-arrival-notice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-arrival-notice-api-openapi.yml
- filename: hmm21-bookings-api-openapi.yml
  format: yaml
  label: HMM Bookings API
  slug: hmm21-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-bookings-api-openapi.yml
- filename: hmm21-eblcompany-id-requests-api-openapi.yml
  format: yaml
  label: HMM Eblcompany Id Requests API
  slug: hmm21-eblcompany-id-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-eblcompany-id-requests-api-openapi.yml
- filename: hmm21-kr-nexawave-cert-file-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CERT FILE API
  slug: hmm21-kr-nexawave-cert-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cert-file-api-openapi.yml
- filename: hmm21-kr-nexawave-class-survey-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CLASS SURVEY API
  slug: hmm21-kr-nexawave-class-survey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-class-survey-api-openapi.yml
- filename: hmm21-kr-nexawave-cms-pms-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CMS PMS API
  slug: hmm21-kr-nexawave-cms-pms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cms-pms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hmm21.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.hmm21.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hmm21 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HMM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HMM
provider_slug: hmm21
slug: hmm21-domain-security
source_filename: hmm21-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hmm21.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hmm21.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hmm21/security/hmm21-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Shipping
- Logistics
- Container Shipping
- Maritime
- DCSA
- Supply Chain
---
