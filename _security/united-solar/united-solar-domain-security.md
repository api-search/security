---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unitedsolarholding.com
  spf: true
hosts:
- cert_expires: Mar 11 01:53:32 2027 GMT
  host: www.unitedsolarholding.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: United Solar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Solar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: United Solar
provider_slug: united-solar
slug: united-solar-domain-security
source_filename: united-solar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitedsolarholding.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 11 01:53:32 2027 GMT\n  hsts: false\ndomains:\n- domain: unitedsolarholding.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-solar/refs/heads/main/security/united-solar-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Solar
- Polysilicon
- Clean Energy
- Manufacturing
- Photovoltaics
- Renewable Energy
---
