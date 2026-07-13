---
api_specs:
- filename: iso-20022-message-definitions
  format: yaml
  label: ISO 20022 Message Catalogue API
  slug: iso-20022-message-catalogue-api
  spec_type: OpenAPI
  url: https://www.iso20022.org/iso-20022-message-definitions
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iso20022.org
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.iso20022.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iso20022 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISO 20022, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ISO 20022
provider_slug: iso20022
slug: iso20022-domain-security
source_filename: iso20022-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iso20022.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: iso20022.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iso20022/refs/heads/main/security/iso20022-domain-security.yml
summary_line: TLSv1.3
tags:
- Financial Messaging
- Payments
- Securities
- Banking
- ISO Standard
- SWIFT
- Financial Services
---
