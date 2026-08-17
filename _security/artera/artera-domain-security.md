---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artera.io
  spf: true
hosts:
- cert_expires: Nov 10 23:16:08 2026 GMT
  host: artera.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: knowledge.artera.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 17:18:42 2026 GMT
  host: api.artera.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Jan 27 16:11:27 2026 GMT
  cert_issuer: Go Daddy Secure Certificate Authority - G2
  cert_subject: CN=apidocs.artera.io
  cert_valid_from: Jan 27 16:11:27 2025 GMT
  finding: EXPIRED TLS CERTIFICATE. This is the developer-portal host Artera prints in its own public knowledge base (https://apidocs.artera.io/docs/0dbfeef0-de7e-4dee-8435-09c5cffd7ed1/specification and https://apidocs.artera.io/login). Every HTTPS request fails certificate validation with "certificate has expired"; the certificate lapsed 2026-01-27, roughly 6.5 months before this probe. The portal is reachable only over plain http://, which then redirects to https://apidocs.artera.app/docs. A developer following Artera's documented link in a browser or any TLS-validating client hits a certificate error on the front door of the API program.
  host: apidocs.artera.io
  hsts: null
  https: false
  method: openssl s_client
  probed: '2026-08-15'
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Artera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artera, probed live across 4 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artera
provider_slug: artera
slug: artera-domain-security
source_filename: artera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:16:08 2026 GMT\n  hsts: false\n- host: knowledge.artera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.artera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:18:42 2026 GMT\n  hsts: null\n- host: apidocs.artera.io\n  https: false\n  tls_version: null\n  cert_expires: Jan 27 16:11:27 2026 GMT\n  cert_expired: true\n  cert_subject: CN=apidocs.artera.io\n  cert_issuer: Go Daddy Secure Certificate Authority - G2\n  cert_valid_from: Jan 27 16:11:27 2025 GMT\n  hsts: null\n  finding: >-\n    EXPIRED TLS CERTIFICATE. This is the developer-portal host Artera prints in\n    its own public knowledge base\n    (https://apidocs.artera.io/docs/0dbfeef0-de7e-4dee-8435-09c5cffd7ed1/specification\n\
  \    and https://apidocs.artera.io/login). Every HTTPS request fails certificate\n    validation with \"certificate has expired\"; the certificate lapsed 2026-01-27,\n    roughly 6.5 months before this probe. The portal is reachable only over plain\n    http://, which then redirects to https://apidocs.artera.app/docs. A developer\n    following Artera's documented link in a browser or any TLS-validating client\n    hits a certificate error on the front door of the API program.\n  probed: '2026-08-15'\n  method: openssl s_client\ndomains:\n- domain: artera.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artera/refs/heads/main/security/artera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Patient Communication
- Patient Engagement
- Health IT
- EHR Integration
- FHIR
- Agentic AI
---
