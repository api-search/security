---
api_specs:
- filename: firehydrant-openapi.yml
  format: yaml
  label: FireHydrant
  slug: firehydrant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 iodef "mailto:ops@firehydrant.io"
  - 0 issue "letsencrypt.org"
  - 0 issue "Digicert.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firehydrant.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "Digicert.com"
  - 0 issue "Digicert.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:ops@firehydrant.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firehydrant.io
  spf: true
hosts:
- cert_expires: Sep  2 22:23:50 2026 GMT
  host: firehydrant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 08:20:53 2026 GMT
  host: api.firehydrant.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firehydrant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FireHydrant, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FireHydrant
provider_slug: firehydrant
slug: firehydrant-domain-security
source_filename: firehydrant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firehydrant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firehydrant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 08:20:53 2026 GMT\n  hsts: null\ndomains:\n- domain: firehydrant.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 iodef \"mailto:ops@firehydrant.io\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"Digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: firehydrant.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"Digicert.com\"\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:ops@firehydrant.io\"\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/security/firehydrant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Incident Management
---
