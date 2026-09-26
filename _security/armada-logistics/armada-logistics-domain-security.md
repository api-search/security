---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: armada-logistics.com
  spf: true
hosts:
- cert_expires: Oct 28 15:34:41 2026 GMT
  host: armada-logistics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Armada Logistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armada Logistics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Armada Logistics
provider_slug: armada-logistics
slug: armada-logistics-domain-security
source_filename: armada-logistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: armada-logistics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:34:41 2026 GMT\n  hsts: false\ndomains:\n- domain: armada-logistics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armada-logistics/refs/heads/main/security/armada-logistics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Freight
- Shipping
- Indonesia
---
