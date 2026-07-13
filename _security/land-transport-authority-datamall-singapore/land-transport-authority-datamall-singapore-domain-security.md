---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lta.gov.sg
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: datamall.lta.gov.sg
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Land Transport Authority Datamall Singapore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Land Transport Authority DataMall, Singapore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Land Transport Authority DataMall, Singapore
provider_slug: land-transport-authority-datamall-singapore
slug: land-transport-authority-datamall-singapore-domain-security
source_filename: land-transport-authority-datamall-singapore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datamall.lta.gov.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lta.gov.sg\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/land-transport-authority-datamall-singapore/refs/heads/main/security/land-transport-authority-datamall-singapore-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
