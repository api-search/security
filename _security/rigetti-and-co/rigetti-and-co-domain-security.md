---
api_specs:
- filename: rigetti-and-co-qcs-openapi.yml
  format: yaml
  label: Rigetti QCS API
  slug: rigetti-qcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rigetti-and-co/refs/heads/main/openapi/rigetti-and-co-qcs-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:postmaster@rigetti.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rigetti.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.qcs.rigetti.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rigetti And Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rigetti & Co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rigetti & Co
provider_slug: rigetti-and-co
slug: rigetti-and-co-domain-security
source_filename: rigetti-and-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.qcs.rigetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: rigetti.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:postmaster@rigetti.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rigetti-and-co/refs/heads/main/security/rigetti-and-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Quantum Computing
- Quantum
- Infrastructure
- Developers
- Cloud Computing
- QPU
- API
---
