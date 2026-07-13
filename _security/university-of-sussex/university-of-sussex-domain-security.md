---
api_specs:
- filename: university-of-sussex-figshare-repository.yaml
  format: yaml
  label: University of Sussex Research Repository (Figshare)
  slug: figshare-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-figshare-repository.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sussex.ac.uk
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: figshare.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.sussex.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: sussex.figshare.com
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
name: University Of Sussex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Sussex, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Sussex
provider_slug: university-of-sussex
slug: university-of-sussex-domain-security
source_filename: university-of-sussex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sussex.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: sussex.figshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.figshare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sussex.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: figshare.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/security/university-of-sussex-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- United Kingdom
---
