---
api_specs:
- filename: circle-pharma-content-openapi.yml
  format: yaml
  label: Circle Pharma Content API
  slug: circle-pharma-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: circlepharma.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep  7 08:13:01 2026 GMT
  host: circlepharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circle Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circle Pharma, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circle Pharma
provider_slug: circle-pharma
slug: circle-pharma-domain-security
source_filename: circle-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circlepharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:13:01 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: circlepharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/security/circle-pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- oncology
- drug-discovery
- macrocycles
- clinical-trials
- life-sciences
- content-api
---
