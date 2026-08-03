---
api_specs:
- filename: fortanix-dsm-openapi-original.json
  format: json
  label: Fortanix Data Security Manager REST API
  slug: dsm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-dsm-openapi-original.json
- filename: fortanix-ccm-openapi-original.json
  format: json
  label: Fortanix Confidential Computing Manager REST API
  slug: ccm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-ccm-openapi-original.json
- filename: fortanix-armor-key-insight-openapi-original.json
  format: json
  label: Fortanix Armor and Key Insight API
  slug: armor-key-insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-armor-key-insight-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fortanix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: smartkey.io
  spf: false
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.fortanix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 09:16:32 2026 GMT
  host: support.fortanix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: amer.smartkey.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortanix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortanix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fortanix
provider_slug: fortanix
slug: fortanix-domain-security
source_filename: fortanix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fortanix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.fortanix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 09:16:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: amer.smartkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fortanix.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: smartkey.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/security/fortanix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Encryption
- Key Management
- Cryptography
- Confidential Computing
- HSM
- Data Security
- Post-Quantum
- Secrets Management
---
