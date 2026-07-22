---
api_specs:
- filename: perimeter-81-openapi-original.json
  format: json
  label: Harmony SASE Public API
  slug: harmony-sase-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perimeter-81/refs/heads/main/openapi/perimeter-81-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perimeter81.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.perimeter81.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 05:39:41 2026 GMT
  host: support.perimeter81.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.perimeter81.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perimeter 81 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perimeter 81, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perimeter 81
provider_slug: perimeter-81
slug: perimeter-81-domain-security
source_filename: perimeter-81-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perimeter81.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: support.perimeter81.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:39:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perimeter81.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: perimeter81.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perimeter-81/refs/heads/main/security/perimeter-81-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- SASE
- Zero Trust
- Networking
- VPN
- ZTNA
- Security
- Cloud Security
---
