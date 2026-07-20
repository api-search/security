---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: growatt.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: showdoc.com.cn
  spf: true
hosts:
- host: growatt.com
  https: false
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: openapi.growatt.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 17:41:51 2026 GMT
  host: www.showdoc.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Growatt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Growatt, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Growatt
provider_slug: growatt
slug: growatt-domain-security
source_filename: growatt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: growatt.com\n  https: false\n- host: openapi.growatt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n- host: www.showdoc.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 17:41:51 2026 GMT\n  hsts: false\ndomains:\n- domain: growatt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: showdoc.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growatt/refs/heads/main/security/growatt-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer Technology
- Solar
- Energy
- Photovoltaic
- Inverters
- Energy Storage
- IoT
- Monitoring
---
