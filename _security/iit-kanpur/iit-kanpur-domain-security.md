---
api_specs:
- filename: oai.pl
  format: yaml
  label: PKK Library OAI-PMH
  slug: library-oai-pmh
  spec_type: OpenAPI
  url: https://libserv.iitk.ac.in/cgi-bin/koha/oai.pl?verb=Identify
- filename: iit-kanpur-library-rest.yaml
  format: yaml
  label: PKK Library Koha ILS-DI
  slug: library-ils-di
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iit-kanpur/refs/heads/main/openapi/iit-kanpur-library-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iitk.ac.in
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.iitk.ac.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: libserv.iitk.ac.in
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Iit Kanpur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Institute of Technology Kanpur, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Indian Institute of Technology Kanpur
provider_slug: iit-kanpur
slug: iit-kanpur-domain-security
source_filename: iit-kanpur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iitk.ac.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: libserv.iitk.ac.in\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: iitk.ac.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-kanpur/refs/heads/main/security/iit-kanpur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- India
- Open Access
- Library
- Metadata
---
