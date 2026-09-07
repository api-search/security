---
api_specs:
- filename: accredify0604-nexus-auth-openapi.yaml
  format: yaml
  label: Accredify Nexus API
  slug: accredify0604-nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-nexus-auth-openapi.yaml
- filename: accredify0604-dashboard-v1-openapi.yaml
  format: yaml
  label: Accredify Dashboard API
  slug: accredify0604-dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-dashboard-v1-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accredify.io
  spf: true
hosts:
- cert_expires: Oct 12 04:36:19 2026 GMT
  host: www.accredify.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:41:49 2026 GMT
  host: docs.nexus.accredify.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: nexus.accredify.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accredify0604 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accredify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Accredify
provider_slug: accredify0604
slug: accredify0604-domain-security
source_filename: accredify0604-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accredify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:36:19 2026 GMT\n  hsts: false\n- host: docs.nexus.accredify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:41:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: nexus.accredify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accredify.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/security/accredify0604-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Verifiable Credentials
- Digital Credentials
- Identity
- Document Verification
- Credentialing
- Education
- Healthcare
- Trust
- OpenBadges
- OID4VCI
- Singapore
---
