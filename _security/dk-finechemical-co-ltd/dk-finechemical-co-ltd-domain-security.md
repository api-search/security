---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dkfinechem.com
  spf: true
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: dkfinechem.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dk Finechemical Co Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DK Finechemical Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DK Finechemical Co., Ltd.
provider_slug: dk-finechemical-co-ltd
slug: dk-finechemical-co-ltd-domain-security
source_filename: dk-finechemical-co-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dkfinechem.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dkfinechem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dk-finechemical-co-ltd/refs/heads/main/security/dk-finechemical-co-ltd-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
