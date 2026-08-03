---
api_specs:
- filename: celsius-network-partner-api-openapi.yml
  format: yaml
  label: Celsius Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/openapi/celsius-network-partner-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:devops@celsius.network"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: celsius.network
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
hosts:
- cert_expires: Sep 15 11:57:08 2026 GMT
  host: celsius.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 09:01:44 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: wallet-api.celsius.network
  https: false
kind: domain-security
layout: security
method: probed
name: Celsius Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celsius Network, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Celsius Network
provider_slug: celsius-network
slug: celsius-network-domain-security
source_filename: celsius-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celsius.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:57:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:01:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wallet-api.celsius.network\n  https: false\ndomains:\n- domain: celsius.network\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:devops@celsius.network\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\
  \n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celsius-network/refs/heads/main/security/celsius-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Financial Services
- Lending
- Custody
- Wallet
- Interest
- KYC
- Retired
---
