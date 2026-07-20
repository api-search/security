---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jupiterone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jupiterone.io
  spf: true
hosts:
- cert_expires: Sep 24 08:43:14 2026 GMT
  host: www.jupiterone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 20:47:48 2026 GMT
  host: docs.jupiterone.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: graphql.us.jupiterone.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jupiterone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JupiterOne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JupiterOne
provider_slug: jupiterone
slug: jupiterone-domain-security
source_filename: jupiterone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jupiterone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:43:14 2026 GMT\n  hsts: null\n- host: docs.jupiterone.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:47:48 2026 GMT\n  hsts: null\n- host: graphql.us.jupiterone.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jupiterone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: jupiterone.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiterone/refs/heads/main/security/jupiterone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- CAASM
- Cyber Asset Management
- Attack Surface Management
- Cloud Security
- Graph
- GraphQL
- Compliance
- Asset Intelligence
---
