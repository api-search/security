---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloombergtax.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: pro.bloombergtax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.bloombergtax.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bloomberg Tax Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg Tax Research, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg Tax Research
provider_slug: bloomberg-tax-research
slug: bloomberg-tax-research-domain-security
source_filename: bloomberg-tax-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pro.bloombergtax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bloombergtax.com\n  https: false\ndomains:\n- domain: bloombergtax.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-tax-research/refs/heads/main/security/bloomberg-tax-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tax Research
- Federal Tax
- State Tax
- International Tax
- Tax Analysis
- Bloomberg Tax
---
