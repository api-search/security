---
api_specs:
- filename: victoria-university-of-wellington-website-globalobject-openapi.yml
  format: yaml
  label: Website Global Object
  slug: website-global-object
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-website-globalobject-openapi.yml
- filename: victoria-university-of-wellington-identity-federation-openapi.yml
  format: yaml
  label: Shibboleth Identity Provider (Tuakiri / eduGAIN)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-identity-federation-openapi.yml
- filename: victoria-university-of-wellington-institutional-repository-openapi.yml
  format: yaml
  label: Institutional Repository (self-hosted DSpace)
  slug: institutional-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/openapi/victoria-university-of-wellington-institutional-repository-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wgtn.ac.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tuakiri.ac.nz
  spf: true
hosts:
- cert_expires: Oct 21 17:02:41 2026 GMT
  host: www.wgtn.ac.nz
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 17 07:30:51 2026 GMT
  host: tuakiri.ac.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: idp.vuw.ac.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wgtn.ac.nz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 17:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: tuakiri.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 07:30:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: idp.vuw.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wgtn.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tuakiri.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/victoria-university-of-wellington/refs/heads/main/security/victoria-university-of-wellington-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- New Zealand
- Public Research University
- Research
- Open Access
- Research Repository
- Institutional Repository
- OAI-PMH
- DSpace
- Library
- Course Catalog
- Identity Federation
- Research Computing
---
