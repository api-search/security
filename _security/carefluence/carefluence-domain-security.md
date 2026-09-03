---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Carefluence Open API R4
  slug: openapi-r4
  spec_type: Postman
  url: https://api.carefluence.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: carefluence.com
  spf: true
hosts:
- cert_expires: Oct 30 17:37:36 2026 GMT
  host: carefluence.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 14:44:57 2026 GMT
  host: api.carefluence.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: classic.carefluence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: core.carefluence.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: SMART/OpenID authorization server; added by the enrichment pass because it is an apis[].baseURL host the automated probe did not enumerate.
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: fhir.carefluence.com
  hsts: null
  https: true
  note: Alias of the FHIR R4 service base; serves the identical CapabilityStatement.
  tls_version: TLSv1.3
- cert_expires: null
  host: docs.carefluence.com
  hsts: null
  https: false
  note: Dangling custom hostname. CNAMEs to ingress-swaggerhub.com; TLS handshake fails (no certificate presented) and plain HTTP returns Cloudflare error 1001 (DNS resolution error). Nothing is served.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Carefluence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carefluence, probed live across 6 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Carefluence
provider_slug: carefluence
slug: carefluence-domain-security
source_filename: carefluence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carefluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 17:37:36 2026 GMT\n  hsts: false\n- host: api.carefluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 14:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: classic.carefluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: core.carefluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: SMART/OpenID authorization server; added by the enrichment pass because it is an apis[].baseURL host the automated probe did not enumerate.\n- host: fhir.carefluence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n  note: Alias of the FHIR R4 service base; serves the\
  \ identical CapabilityStatement.\n- host: docs.carefluence.com\n  https: false\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  note: >-\n    Dangling custom hostname. CNAMEs to ingress-swaggerhub.com; TLS handshake\n    fails (no certificate presented) and plain HTTP returns Cloudflare error\n    1001 (DNS resolution error). Nothing is served.\ndomains:\n- domain: carefluence.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carefluence/refs/heads/main/security/carefluence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- HL7
- SMART on FHIR
- Electronic Health Records
- Clinical Data
- Health IT
- ONC Certified
- USCDI
- OAuth 2.0
- Telehealth
- Health Information Exchange
---
