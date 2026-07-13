---
api_specs:
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Studios API
  slug: shootproof-studios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Events & Galleries API
  slug: shootproof-events-galleries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Photos API
  slug: shootproof-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Clients API
  slug: shootproof-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Orders API
  slug: shootproof-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Contracts API
  slug: shootproof-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: shootproof.com
  spf: true
hosts:
- cert_expires: Oct  3 10:46:49 2026 GMT
  host: www.shootproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: developer.shootproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.shootproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shootproof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShootProof, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ShootProof
provider_slug: shootproof
slug: shootproof-domain-security
source_filename: shootproof-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shootproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:46:49 2026 GMT\n  hsts: false\n- host: developer.shootproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.shootproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: shootproof.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/security/shootproof-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Photography
- Client Galleries
- Proofing
- Digital Downloads
- Photo Studio Management
- E-Commerce
- SaaS
---
