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
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.dla.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Operation Support Equipment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Operation Support Equipment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Operation Support Equipment
provider_slug: operation-support-equipment
slug: operation-support-equipment-domain-security
source_filename: operation-support-equipment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dla.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\ndomains:\n- domain: dla.mil\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/operation-support-equipment/refs/heads/main/security/operation-support-equipment-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Deployment
- Equipment Management
- Inventory
- Logistics
- Maintenance
- Operation Support
---
