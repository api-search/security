---
api_specs:
- filename: ariregister-rik-ee-beneficialowners-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Beneficial Owners API
  slug: ariregister-rik-ee-beneficialowners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-beneficialowners-api-openapi.yml
- filename: ariregister-rik-ee-company-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Company API
  slug: ariregister-rik-ee-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-company-api-openapi.yml
- filename: ariregister-rik-ee-keylogin-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Key Login API
  slug: ariregister-rik-ee-keylogin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-keylogin-api-openapi.yml
- filename: ariregister-rik-ee-person-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Person API
  slug: ariregister-rik-ee-person-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-person-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rik.ee
  spf: true
hosts:
- cert_expires: Dec 23 00:12:46 2026 GMT
  host: ariregister.rik.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Estonian e-Business Register (RIK) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estonian e-Business Register (RIK), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Estonian e-Business Register (RIK)
provider_slug: ariregister-rik-ee
slug: ariregister-rik-ee-domain-security
source_filename: ariregister-rik-ee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ariregister.rik.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 00:12:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rik.ee\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ariregister-rik-ee/security/ariregister-rik-ee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Business Registry
- Open Data
- Estonia
- Beneficial Ownership
- SOAP
- KYB
---
