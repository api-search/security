---
api_specs:
- filename: mend-platform-openapi-original.json
  format: json
  label: Mend AppSec Platform API
  slug: mend-appsec-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/openapi/mend-platform-openapi-original.json
- filename: mend-sca-openapi-original.json
  format: json
  label: Mend SCA API
  slug: mend-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/openapi/mend-sca-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mend.io
  spf: true
hosts:
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: www.mend.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 02:17:52 2026 GMT
  host: api-docs.mend.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api-saas.mend.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mend
provider_slug: mend
slug: mend-domain-security
source_filename: mend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.mend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:17:52 2026 GMT\n  hsts: false\n- host: api-saas.mend.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/security/mend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Security
- Software Composition Analysis
- SAST
- Container Security
- AI Security
- Dependency Management
- Vulnerability Management
- DevSecOps
- SBOM
- Open Source Security
- Company
---
