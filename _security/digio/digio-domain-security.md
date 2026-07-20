---
api_specs:
- filename: digio-openapi.yml
  format: yaml
  label: Digio eSign API
  slug: digio-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio eMandate (eNACH) API
  slug: digio-emandate-enach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio KYC API
  slug: digio-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
- filename: digio-openapi.yml
  format: yaml
  label: Digio Documents & eStamp API
  slug: digio-documents-estamp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/openapi/digio-openapi.yml
description: ''
domains:
- domain: digio.in
  hosting: AWS (Amazon-issued RSA TLS certificates; ap-south-1 / India region IPs)
  tls: All probed hosts serve HTTPS with valid Amazon-issued certificates.
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.digio.in
  http_status: 404
  https: true
  note: Production API host. Root returns 404 (API-only host, no landing page).
  remote_ip: 13.206.128.149
  tls_issuer: Amazon RSA 2048 M01
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: ext.digio.in
  http_status: 200
  https: true
  note: Sandbox / test API host.
  remote_ip: 65.0.222.86
  tls_issuer: Amazon RSA 2048 M01
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: documentation.digio.in
  http_status: 200
  https: true
  remote_ip: 3.108.92.28
  tls_issuer: Amazon RSA 2048 M01
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.digio.in
  http_status: 200
  https: true
  tls_issuer: Amazon RSA 2048 M04
kind: domain-security
layout: security
method: probed
name: Digio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digio, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Digio
provider_slug: digio
slug: digio-domain-security
source_filename: digio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.digio.in\n  https: true\n  http_status: 404\n  remote_ip: 13.206.128.149\n  tls_issuer: Amazon RSA 2048 M01\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  note: Production API host. Root returns 404 (API-only host, no landing page).\n- host: ext.digio.in\n  https: true\n  http_status: 200\n  remote_ip: 65.0.222.86\n  tls_issuer: Amazon RSA 2048 M01\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  note: Sandbox / test API host.\n- host: documentation.digio.in\n  https: true\n  http_status: 200\n  remote_ip: 3.108.92.28\n  tls_issuer: Amazon RSA 2048 M01\n  cert_expires: Sep 22 23:59:59 2026 GMT\n- host: www.digio.in\n  https: true\n  http_status: 200\n  tls_issuer: Amazon RSA 2048 M04\n  cert_expires: Sep 19 23:59:59 2026 GMT\ndomains:\n- domain: digio.in\n  hosting: AWS (Amazon-issued RSA TLS certificates; ap-south-1 / India region IPs)\n  tls: All probed hosts\
  \ serve HTTPS with valid Amazon-issued certificates.\nnotes: >-\n  Hosts live-probed 2026-07-17. api.digio.in is the production REST API host;\n  ext.digio.in is the sandbox. All traffic is HTTPS; Digio states bank-grade\n  security with 2-factor authentication in its signing and KYC flows.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digio/refs/heads/main/security/digio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- eSign
- KYC
- eNACH
- eMandate
- Digital Signature
- India
- Fintech
- Identity Verification
---
