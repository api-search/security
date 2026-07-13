---
api_specs:
- filename: victoria-university-of-wellington-figshare-rest.yaml
  format: yaml
  label: Figshare REST API (Open Access Repository)
  slug: figshare-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-figshare-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wgtn.ac.nz
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Oct 21 17:02:41 2026 GMT
  host: www.wgtn.ac.nz
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: docs.figshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Victoria University Of Wellington Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Victoria University of Wellington, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Victoria University of Wellington
provider_slug: victoria-university-of-wellington
slug: victoria-university-of-wellington-domain-security
source_filename: victoria-university-of-wellington-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wgtn.ac.nz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 17:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wgtn.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/security/victoria-university-of-wellington-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Library
- New Zealand
---
