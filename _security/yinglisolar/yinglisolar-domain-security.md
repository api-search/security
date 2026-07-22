---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yinglisolar.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.yinglisolar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yinglisolar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for yinglisolar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: yinglisolar
provider_slug: yinglisolar
slug: yinglisolar-domain-security
source_filename: yinglisolar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yinglisolar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: yinglisolar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yinglisolar/refs/heads/main/security/yinglisolar-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Solar
- Photovoltaic
- Renewable Energy
- Manufacturing
- Energy
---
