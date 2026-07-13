---
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dla.mil
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fedmall.mil
  spf: true
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.dla.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.dibbs.bsm.dla.mil
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.fedmall.mil
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Defense Logistics Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Logistics Agency, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Logistics Agency
provider_slug: defense-logistics-agency
slug: defense-logistics-agency-domain-security
source_filename: defense-logistics-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dla.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\n- host: www.dibbs.bsm.dla.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: www.fedmall.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dla.mil\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fedmall.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-logistics-agency/refs/heads/main/security/defense-logistics-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Acquisition
- Defense
- Department of Defense
- DLA
- Federal Government
- Logistics
- Procurement
- Supply Chain
---
