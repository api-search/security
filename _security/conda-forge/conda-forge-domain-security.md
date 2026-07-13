---
api_specs:
- filename: docs
  format: yaml
  label: Anaconda.org Package API
  slug: anacondaorg-package-api
  spec_type: OpenAPI
  url: https://api.anaconda.org/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anaconda.org
  spf: true
hosts:
- cert_expires: Sep 22 19:16:28 2026 GMT
  host: anaconda.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 19:50:00 2026 GMT
  host: api.anaconda.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 19:50:00 2026 GMT
  host: conda.anaconda.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conda Forge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for conda-forge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: conda-forge
provider_slug: conda-forge
slug: conda-forge-domain-security
source_filename: conda-forge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anaconda.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:16:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.anaconda.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: conda.anaconda.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:50:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: anaconda.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conda-forge/refs/heads/main/security/conda-forge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- conda
- packages
- scientific-computing
- python
- open-source
---
