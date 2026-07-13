---
api_specs:
- filename: henchman-openapi.yml
  format: yaml
  label: Henchman Clause and Definition Search
  slug: clause-and-definition-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/openapi/henchman-openapi.yml
- filename: henchman-openapi.yml
  format: yaml
  label: Henchman Knowledge Base
  slug: knowledge-base
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/openapi/henchman-openapi.yml
- filename: henchman-openapi.yml
  format: yaml
  label: Henchman Integrations
  slug: integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/openapi/henchman-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: henchman.io
  spf: true
hosts:
- host: www.henchman.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
- host: henchman.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Henchman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Henchman, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Henchman
provider_slug: henchman
slug: henchman-domain-security
source_filename: henchman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.henchman.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\n- host: henchman.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: henchman.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/henchman/refs/heads/main/security/henchman-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Legal
- Legal Tech
- Contract Drafting
- Clause Search
- Knowledge Management
- AI
---
