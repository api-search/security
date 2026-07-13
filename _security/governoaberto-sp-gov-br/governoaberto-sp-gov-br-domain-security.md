---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sp.gov.br
  spf: true
hosts:
- host: www.governoaberto.sp.gov.br
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.governo'
kind: domain-security
layout: security
method: probed
name: Governoaberto Sp Gov Br Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Governo Aberto do Estado de São Paulo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Governo Aberto do Estado de São Paulo
provider_slug: governoaberto-sp-gov-br
slug: governoaberto-sp-gov-br-domain-security
source_filename: governoaberto-sp-gov-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.governoaberto.sp.gov.br\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.governo'\n  hsts: null\ndomains:\n- domain: sp.gov.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/governoaberto-sp-gov-br/refs/heads/main/security/governoaberto-sp-gov-br-domain-security.yml
summary_line: DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- br
---
