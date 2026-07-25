---
api_specs:
- filename: matrix-account-api-openapi.yml
  format: yaml
  label: Matrix Account API
  slug: matrix-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-account-api-openapi.yml
- filename: matrix-capabilities-api-openapi.yml
  format: yaml
  label: Matrix Capabilities API
  slug: matrix-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-capabilities-api-openapi.yml
- filename: matrix-createroom-api-openapi.yml
  format: yaml
  label: Matrix CreateRoom API
  slug: matrix-createroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-createroom-api-openapi.yml
- filename: matrix-devices-api-openapi.yml
  format: yaml
  label: Matrix Devices API
  slug: matrix-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-devices-api-openapi.yml
- filename: matrix-directory-api-openapi.yml
  format: yaml
  label: Matrix Directory API
  slug: matrix-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-directory-api-openapi.yml
- filename: matrix-join-api-openapi.yml
  format: yaml
  label: Matrix Join API
  slug: matrix-join-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-join-api-openapi.yml
- filename: matrix-keys-api-openapi.yml
  format: yaml
  label: Matrix Keys API
  slug: matrix-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-keys-api-openapi.yml
- filename: matrix-login-api-openapi.yml
  format: yaml
  label: Matrix Login API
  slug: matrix-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-login-api-openapi.yml
- filename: matrix-logout-api-openapi.yml
  format: yaml
  label: Matrix Logout API
  slug: matrix-logout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-logout-api-openapi.yml
- filename: matrix-profile-api-openapi.yml
  format: yaml
  label: Matrix Profile API
  slug: matrix-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-profile-api-openapi.yml
- filename: matrix-publicrooms-api-openapi.yml
  format: yaml
  label: Matrix PublicRooms API
  slug: matrix-publicrooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-publicrooms-api-openapi.yml
- filename: matrix-refresh-api-openapi.yml
  format: yaml
  label: Matrix Refresh API
  slug: matrix-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-refresh-api-openapi.yml
- filename: matrix-register-api-openapi.yml
  format: yaml
  label: Matrix Register API
  slug: matrix-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-register-api-openapi.yml
- filename: matrix-rooms-api-openapi.yml
  format: yaml
  label: Matrix Rooms API
  slug: matrix-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-rooms-api-openapi.yml
- filename: matrix-sync-api-openapi.yml
  format: yaml
  label: Matrix Sync API
  slug: matrix-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-sync-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: matrix.org
  spf: true
hosts:
- cert_expires: Sep 10 12:59:13 2026 GMT
  host: matrix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:46:11 2026 GMT
  host: spec.matrix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matrix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matrix
provider_slug: matrix
slug: matrix-domain-security
source_filename: matrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matrix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spec.matrix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:46:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: matrix.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/security/matrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Decentralized
- Federated
- Open Standard
- Real-Time Communication
- VoIP
---
