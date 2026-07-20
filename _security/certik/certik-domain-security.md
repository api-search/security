---
api_specs:
- filename: certik-skynet-openapi.yml
  format: yaml
  label: CertiK Partner (Skynet) API
  slug: certik-partner-skynet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certik/refs/heads/main/openapi/certik-skynet-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: certik.com
  spf: true
hosts:
- cert_expires: Aug 22 05:59:30 2026 GMT
  host: www.certik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CertiK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CertiK
provider_slug: certik
slug: certik-domain-security
source_filename: certik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:59:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: certik.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certik/refs/heads/main/security/certik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Web3
- Blockchain
- Smart Contract Security
- Security Auditing
- Threat Intelligence
---
