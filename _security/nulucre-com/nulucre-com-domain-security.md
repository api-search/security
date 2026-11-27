---
api_specs:
- filename: nulucre-com-reputation-api-openapi.yml
  format: yaml
  label: Nulucre Reputation API
  slug: nulucre-com-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nulucre-com/openapi/nulucre-com-reputation-api-openapi.yml
- filename: nulucre-com-verify-api-openapi.yml
  format: yaml
  label: Nulucre Verify API
  slug: nulucre-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nulucre-com/openapi/nulucre-com-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "comodoca.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nulucre.com
  spf: true
hosts:
- cert_expires: Feb  1 19:22:41 2027 GMT
  host: nulucre.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nulucre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nulucre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nulucre
provider_slug: nulucre-com
slug: nulucre-com-domain-security
source_filename: nulucre-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nulucre.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 19:22:41 2027 GMT\n  hsts: false\ndomains:\n- domain: nulucre.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nulucre-com/security/nulucre-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Reputation
- Oracle
- Fact-Verification
- Blockchain
- DeFi
---
