---
api_specs:
- filename: openapi.json
  format: json
  label: BenchSci API
  slug: benchsci-api
  spec_type: OpenAPI
  url: https://api.benchsci.com/openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: benchsci.com
  spf: true
hosts:
- cert_expires: Sep  2 17:02:25 2026 GMT
  host: www.benchsci.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 07:03:20 2026 GMT
  host: api.benchsci.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Benchsci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenchSci, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BenchSci
provider_slug: benchsci
slug: benchsci-domain-security
source_filename: benchsci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchsci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:02:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.benchsci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 07:03:20 2026 GMT\n  hsts: null\ndomains:\n- domain: benchsci.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benchsci/refs/heads/main/security/benchsci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Biopharma
- Drug Discovery
- AI
- Reagents
- Antibodies
- Scientific Research
- Life Sciences
- Preclinical Research
---
