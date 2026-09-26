---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: globalp.com
  spf: true
hosts:
- cert_expires: Nov 15 07:19:02 2026 GMT
  host: www.globalp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Mar 30 23:59:59 2024 GMT
  cert_issuer: C=US, O=DigiCert Inc, CN=DigiCert TLS RSA SHA256 2020 CA1
  cert_subject: C=US, ST=Massachusetts, L=Waltham, O=Global Partners LP, CN=*.globalp.com
  chain_incomplete: true
  host: api.globalp.com
  hsts: false
  https: true
  note: Probed 2026-09-12 outside the apis.yml/servers[] host set because the hostname suggested an API. api.globalp.com resolves to 34.233.44.177 and serves, over Apache, a static archived copy of a GitLab Community Edition sign-in page; every GitLab API path (/api/v4/version, /api/v4/projects, /explore) returns an Apache 404, so there is no live API behind it. Its wildcard certificate is genuinely Global Partners LP (O=Global Partners LP, Waltham MA) but EXPIRED on 2024-03-30 and the chain is incomplete — every standard client refuses the connection. Recorded as a live security finding, not as an API surface.
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Global Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Partners LP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Global Partners LP
provider_slug: global-partners
slug: global-partners-domain-security
source_filename: global-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globalp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:19:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.globalp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_subject: C=US, ST=Massachusetts, L=Waltham, O=Global Partners LP, CN=*.globalp.com\n  cert_issuer: C=US, O=DigiCert Inc, CN=DigiCert TLS RSA SHA256 2020 CA1\n  cert_expires: Mar 30 23:59:59 2024 GMT\n  cert_expired: true\n  chain_incomplete: true\n  hsts: false\n  note: Probed 2026-09-12 outside the apis.yml/servers[] host set because the hostname suggested an API. api.globalp.com resolves\n    to 34.233.44.177 and serves, over Apache, a static archived copy of a GitLab Community Edition sign-in page; every GitLab\n    API path (/api/v4/version, /api/v4/projects, /explore) returns an Apache 404, so there is no live API behind it. Its wildcard\n    certificate\
  \ is genuinely Global Partners LP (O=Global Partners LP, Waltham MA) but EXPIRED on 2024-03-30 and the chain\n    is incomplete — every standard client refuses the connection. Recorded as a live security finding, not as an API surface.\ndomains:\n- domain: globalp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-partners/refs/heads/main/security/global-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Fuel Distribution
- Oil and Gas
- Petroleum
- Retail Fuel
- Terminal
- Fortune 500
- WordPress
- Terminal Network
- Retail Locations
---
