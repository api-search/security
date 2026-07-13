---
api_specs:
- filename: $metadata
  format: yaml
  label: WHO GHO OData API
  slug: who-gho-odata-api
  spec_type: OpenAPI
  url: https://ghoapi.azureedge.net/api/$metadata
- filename: index.html
  format: yaml
  label: WHO ICD API
  slug: who-icd-api
  spec_type: OpenAPI
  url: https://id.who.int/swagger/index.html
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: who.int
  spf: true
- caa:
  - 0 issue "microsoft.com"
  - 0 issuewild "microsoft.com"
  - 0 issue "digicert.com; account=488f180f66637f6181c0f055bdfe0e1c40852d9cc7ac5affded3c97e2fab3f1e"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com; account=37519e363bd0f3f470682383a25b2daa13232906ff77b9eb03d1269486782a2a"
  - 0 issue "digicert.com; account=4735470c395ee719a2a0c2a15a49193ff5add1d47d164d31d186797e73892a18"
  dmarc: false
  dnssec: false
  domain: azureedge.net
  spf: false
hosts:
- cert_expires: Aug 31 14:46:05 2026 GMT
  host: www.who.int
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 05:48:59 2026 GMT
  host: ghoapi.azureedge.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 09:58:40 2026 GMT
  host: icd.who.int
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Who Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Health Organization (WHO), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World Health Organization (WHO)
provider_slug: who
slug: who-domain-security
source_filename: who-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.who.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:46:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ghoapi.azureedge.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 05:48:59 2026 GMT\n  hsts: null\n- host: icd.who.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 09:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: who.int\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azureedge.net\n  dnssec: false\n  caa:\n  - 0 issue \"microsoft.com\"\n  - 0 issuewild \"microsoft.com\"\n  - 0 issue \"digicert.com; account=488f180f66637f6181c0f055bdfe0e1c40852d9cc7ac5affded3c97e2fab3f1e\"\
  \n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com; account=37519e363bd0f3f470682383a25b2daa13232906ff77b9eb03d1269486782a2a\"\n  - 0 issue \"digicert.com; account=4735470c395ee719a2a0c2a15a49193ff5add1d47d164d31d186797e73892a18\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/who/refs/heads/main/security/who-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Global Health
- Disease Surveillance
- Immunization
- Health Statistics
- ICD
- WHO
- United Nations
- Open Data
---
