---
api_specs:
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Vault Tokenization API
  slug: vgs-vault-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Accounts Management API
  slug: vgs-accounts-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Routes & Proxy API
  slug: vgs-routes-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Functions API
  slug: vgs-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Organizations API
  slug: vgs-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@verygoodsecurity.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: verygoodsecurity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: verygoodvault.com
  spf: false
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: www.verygoodsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.sandbox.verygoodvault.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 14 02:45:30 2026 GMT
  host: docs.verygoodsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vgs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Very Good Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Very Good Security
provider_slug: vgs
slug: vgs-domain-security
source_filename: vgs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verygoodsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sandbox.verygoodvault.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: docs.verygoodsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:45:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verygoodsecurity.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admin@verygoodsecurity.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: verygoodvault.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/security/vgs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Tokenization
- Data Privacy
- PCI Compliance
- Vault
---
