---
api_specs:
- filename: openapi.json
  format: json
  label: Prisma Data Platform API
  slug: prisma-data-platform-api
  spec_type: OpenAPI
  url: https://api.cloud.prisma.io/openapi.json
- filename: prisma-accelerate-openapi.yml
  format: yaml
  label: Prisma Accelerate API
  slug: prisma-accelerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-accelerate-openapi.yml
- filename: prisma-pulse-openapi.yml
  format: yaml
  label: Prisma Pulse API
  slug: prisma-pulse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-pulse-openapi.yml
- filename: prisma-postgres-management-openapi.yml
  format: yaml
  label: Prisma Postgres Management API
  slug: prisma-postgres-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-postgres-management-openapi.yml
- filename: prisma-client-openapi.yml
  format: yaml
  label: Prisma Client API
  slug: prisma-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-client-openapi.yml
- filename: prisma-optimize-openapi.yml
  format: yaml
  label: Prisma Optimize API
  slug: prisma-optimize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/openapi/prisma-optimize-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@prisma.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prisma.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: prisma-data.net
  spf: false
hosts:
- cert_expires: Sep  8 04:32:42 2026 GMT
  host: console.prisma.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:35:34 2026 GMT
  host: www.prisma.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:15:34 2026 GMT
  host: accelerate.prisma-data.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prisma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prisma, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prisma
provider_slug: prisma
slug: prisma-domain-security
source_filename: prisma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.prisma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:32:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.prisma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:35:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: accelerate.prisma-data.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:15:34 2026 GMT\n  hsts: null\ndomains:\n- domain: prisma.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@prisma.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: prisma-data.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/security/prisma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
