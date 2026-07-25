---
api_specs:
- filename: gluu-discovery-api-openapi.yml
  format: yaml
  label: Gluu discovery API
  slug: gluu-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-discovery-api-openapi.yml
- filename: gluu-fido-api-openapi.yml
  format: yaml
  label: Gluu fido API
  slug: gluu-fido-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-fido-api-openapi.yml
- filename: gluu-groups-api-openapi.yml
  format: yaml
  label: Gluu groups API
  slug: gluu-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-groups-api-openapi.yml
- filename: gluu-users-api-openapi.yml
  format: yaml
  label: Gluu users API
  slug: gluu-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/openapi/gluu-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gluu.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jans.io
  spf: true
hosts:
- cert_expires: Sep 14 07:15:44 2026 GMT
  host: gluu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 21:39:18 2026 GMT
  host: docs.gluu.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 05:06:10 2026 GMT
  host: jans.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gluu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gluu, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gluu
provider_slug: gluu
slug: gluu-domain-security
source_filename: gluu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gluu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:15:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gluu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:39:18 2026 GMT\n  hsts: false\n- host: jans.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 05:06:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gluu.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jans.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/security/gluu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Management
- Authentication
- Authorization
- IAM
- Identities
- OAuth
- OpenID Connect
---
