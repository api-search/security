---
api_specs:
- filename: loughborough-research-repository-rest.yaml
  format: yaml
  label: Loughborough Research Repository (figshare REST API)
  slug: research-repository-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/openapi/loughborough-research-repository-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lboro.ac.uk
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.lboro.ac.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: docs.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Loughborough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loughborough University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Loughborough University
provider_slug: loughborough
slug: loughborough-domain-security
source_filename: loughborough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lboro.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lboro.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loughborough/refs/heads/main/security/loughborough-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research Data
- Open Access
- Repository
- Identity
---
