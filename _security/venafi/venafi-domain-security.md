---
api_specs:
- filename: venafi-certificate-manager-saas-openapi.yml
  format: yaml
  label: Certificate Manager - SaaS API (Venafi Control Plane)
  slug: certificate-manager-saas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-certificate-manager-saas-openapi.yml
- filename: venafi-trust-protection-foundation-websdk-openapi.yml
  format: yaml
  label: Trust Protection Foundation WebSDK (Venafi Trust Protection Platform)
  slug: trust-protection-foundation-websdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/openapi/venafi-trust-protection-foundation-websdk-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: venafi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: venafi.cloud
  spf: true
hosts:
- cert_expires: Nov 15 18:51:50 2026 GMT
  host: venafi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 10:30:37 2026 GMT
  host: developer.venafi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.venafi.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Venafi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Venafi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Venafi
provider_slug: venafi
slug: venafi-domain-security
source_filename: venafi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venafi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 18:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.venafi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 10:30:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.venafi.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: venafi.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: venafi.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venafi/refs/heads/main/security/venafi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Certificates
- PKI
- Machine Identity
- Identity
- Cryptography
- Key Management
- Certificate Lifecycle Management
- DevOps
- Kubernetes
- Code Signing
---
