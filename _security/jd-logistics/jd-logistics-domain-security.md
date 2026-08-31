---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jdl.com
  spf: true
hosts:
- cert_expires: Feb 28 01:16:19 2027 GMT
  host: www.jdl.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jd Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JD Logistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JD Logistics
provider_slug: jd-logistics
slug: jd-logistics-domain-security
source_filename: jd-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jdl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 01:16:19 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: jdl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jd-logistics/refs/heads/main/security/jd-logistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Shipping
- Fulfillment
- Warehousing
- Delivery
- Cold Chain
- Cross Border
- E-Commerce
---
