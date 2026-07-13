---
api_specs:
- filename: imperial-college-london-spiral.yaml
  format: yaml
  label: Spiral Open Access Repository
  slug: spiral
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperial-college-london/refs/heads/main/openapi/imperial-college-london-spiral.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: imperial.ac.uk
  spf: true
hosts:
- cert_expires: Sep 24 23:23:30 2026 GMT
  host: www.imperial.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: spiral.imperial.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imperial College London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imperial College London, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Imperial College London
provider_slug: imperial-college-london
slug: imperial-college-london-domain-security
source_filename: imperial-college-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imperial.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:23:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spiral.imperial.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imperial.ac.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperial-college-london/refs/heads/main/security/imperial-college-london-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- United Kingdom
- Open Access
- Repository
- Identity
---
