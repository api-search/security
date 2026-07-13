---
api_specs:
- filename: ruckus-one-api-openapi.yml
  format: yaml
  label: RUCKUS One API
  slug: ruckus-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/openapi/ruckus-one-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commscope.com
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: ruckus.cloud
  spf: false
hosts:
- cert_expires: Oct  5 01:24:02 2026 GMT
  host: www.commscope.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:02:31 2026 GMT
  host: docs.ruckus.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 19:30:43 2026 GMT
  host: api.ruckus.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commscope Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CommScope Holding, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CommScope Holding
provider_slug: commscope-holding
slug: commscope-holding-domain-security
source_filename: commscope-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 01:24:02 2026 GMT\n  hsts: false\n- host: docs.ruckus.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:02:31 2026 GMT\n  hsts: false\n- host: api.ruckus.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:30:43 2026 GMT\n  hsts: null\ndomains:\n- domain: commscope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ruckus.cloud\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/security/commscope-holding-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Access Points
- Cabling
- Connectivity
- ICX Switches
- Infrastructure
- Networking
- RUCKUS
- Wi-Fi
- Fortune 1000
---
