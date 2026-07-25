---
api_specs:
- filename: interhyp-commands-api-openapi.yml
  format: yaml
  label: Interhyp commands API
  slug: interhyp-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-commands-api-openapi.yml
- filename: interhyp-documents-api-openapi.yml
  format: yaml
  label: Interhyp documents API
  slug: interhyp-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-documents-api-openapi.yml
- filename: interhyp-financing-application-api-openapi.yml
  format: yaml
  label: Interhyp financing-application API
  slug: interhyp-financing-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-financing-application-api-openapi.yml
- filename: interhyp-info-api-openapi.yml
  format: yaml
  label: Interhyp info API
  slug: interhyp-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-info-api-openapi.yml
- filename: interhyp-logbook-api-openapi.yml
  format: yaml
  label: Interhyp logbook API
  slug: interhyp-logbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-logbook-api-openapi.yml
- filename: interhyp-pre-submission-checks-api-openapi.yml
  format: yaml
  label: Interhyp pre-submission-checks API
  slug: interhyp-pre-submission-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-pre-submission-checks-api-openapi.yml
- filename: interhyp-protocol-api-openapi.yml
  format: yaml
  label: Interhyp protocol API
  slug: interhyp-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-protocol-api-openapi.yml
- filename: interhyp-submissions-api-openapi.yml
  format: yaml
  label: Interhyp submissions API
  slug: interhyp-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/openapi/interhyp-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ehyphome.de
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: interhyp.de
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: developer.ehyphome.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.interhyp.de
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: api-test.interhyp.de
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Interhyp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interhyp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Interhyp
provider_slug: interhyp
slug: interhyp-domain-security
source_filename: interhyp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ehyphome.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.interhyp.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\n- host: api-test.interhyp.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ehyphome.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: interhyp.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interhyp/refs/heads/main/security/interhyp-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Mortgage
- Lending
- Baufinanzierung
- Real Estate
- Banking
- Germany
- API First
---
