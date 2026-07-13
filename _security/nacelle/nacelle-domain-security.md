---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: nacelle.com
  spf: true
hosts:
- cert_expires: Sep 13 19:15:48 2026 GMT
  host: nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:01:32 2026 GMT
  host: docs.nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: storefront.api.nacelle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nacelle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nacelle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nacelle
provider_slug: nacelle
slug: nacelle-domain-security
source_filename: nacelle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: storefront.api.nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nacelle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/security/nacelle-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- GraphQL
- Content
- Data Indexing
---
