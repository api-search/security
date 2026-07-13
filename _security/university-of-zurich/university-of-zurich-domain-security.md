---
api_specs:
- filename: university-of-zurich-eduid-oidc.yaml
  format: yaml
  label: SWITCH edu-ID / UZH Identity (SAML & OpenID Connect)
  slug: eduid-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/openapi/university-of-zurich-eduid-oidc.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uzh.ch
  spf: true
hosts:
- host: www.uzh.ch
  https: false
- cert_expires: Aug 12 22:49:30 2026 GMT
  host: www.zora.uzh.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.zi.uzh.ch
  https: false
kind: domain-security
layout: security
method: probed
name: University Of Zurich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Zurich, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Zurich
provider_slug: university-of-zurich
slug: university-of-zurich-domain-security
source_filename: university-of-zurich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uzh.ch\n  https: false\n- host: www.zora.uzh.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:49:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zi.uzh.ch\n  https: false\ndomains:\n- domain: uzh.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/security/university-of-zurich-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Switzerland
- Open Access
- Research Repository
- Open Data
- Identity
---
