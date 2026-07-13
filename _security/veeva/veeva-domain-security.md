---
api_specs:
- filename: veeva-vault-openapi.yml
  format: yaml
  label: Veeva Vault Platform API
  slug: veeva-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-vault-openapi.yml
- filename: veeva-vault-openapi.yml
  format: yaml
  label: Veeva Vault Query Language (VQL) API
  slug: veeva-vault-query-language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/openapi/veeva-vault-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veeva.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "thawte.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veevavault.com
  spf: true
hosts:
- cert_expires: Aug 27 15:10:08 2026 GMT
  host: www.veeva.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: developer.veevavault.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: myvault.veevavault.com
  https: false
kind: domain-security
layout: security
method: probed
name: Veeva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for veeva, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: veeva
provider_slug: veeva
slug: veeva-domain-security
source_filename: veeva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:10:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.veevavault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\n- host: myvault.veevavault.com\n  https: false\ndomains:\n- domain: veeva.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: veevavault.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"thawte.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n \
  \ dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/security/veeva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
