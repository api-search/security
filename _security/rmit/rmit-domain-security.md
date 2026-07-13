---
api_specs:
- filename: rmit-figshare-api.yaml
  format: yaml
  label: RMIT Research Data (Figshare REST API)
  slug: figshare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/openapi/rmit-figshare-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rmit.edu.au
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.rmit.edu.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: rmit.figshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rmit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RMIT University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RMIT University
provider_slug: rmit
slug: rmit-domain-security
source_filename: rmit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rmit.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rmit.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rmit.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rmit/refs/heads/main/security/rmit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Australia
---
