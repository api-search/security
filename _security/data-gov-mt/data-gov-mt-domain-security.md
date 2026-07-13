---
description: ''
domains:
- caa:
  - cloudproxy.gov.mt.
  dmarc: false
  dnssec: true
  domain: data.gov.mt
  spf: false
hosts:
- cert_expires: Oct  1 09:12:31 2026 GMT
  host: portal.data.gov.mt
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 09:12:31 2026 GMT
  host: msdi.data.gov.mt
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Gov Mt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.gov.mt (Open Data Malta), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: data.gov.mt (Open Data Malta)
provider_slug: data-gov-mt
slug: data-gov-mt-domain-security
source_filename: data-gov-mt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.data.gov.mt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:12:31 2026 GMT\n  hsts: null\n- host: msdi.data.gov.mt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:12:31 2026 GMT\n  hsts: null\ndomains:\n- domain: data.gov.mt\n  dnssec: true\n  caa:\n  - cloudproxy.gov.mt.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-gov-mt/refs/heads/main/security/data-gov-mt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Open Data
- Custom Platform
- DCAT-AP
- Government Data
- National Government
- Malta
- Europe
---
