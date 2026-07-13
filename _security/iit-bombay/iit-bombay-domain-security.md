---
api_specs:
- filename: request
  format: yaml
  label: DSpace Institutional Repository OAI-PMH
  slug: dspace-oai-pmh
  spec_type: OpenAPI
  url: https://dspace.library.iitb.ac.in/oai/request?verb=Identify
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iitb.ac.in
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tech-iitb.org
  spf: false
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.iitb.ac.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 15:26:03 2027 GMT
  host: gymkhana.iitb.ac.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 18:25:35 2026 GMT
  host: sso.tech-iitb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iit Bombay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Technology Bombay, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Indian Institute of Technology Bombay
provider_slug: iit-bombay
slug: iit-bombay-domain-security
source_filename: iit-bombay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iitb.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gymkhana.iitb.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 15:26:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sso.tech-iitb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:25:35 2026 GMT\n  hsts: false\ndomains:\n- domain: iitb.ac.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tech-iitb.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/security/iit-bombay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- India
- Open Access
- Identity
---
