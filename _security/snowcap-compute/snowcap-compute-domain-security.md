---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: snowcapcompute.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.snowcapcompute.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snowcap Compute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snowcap Compute, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Snowcap Compute
provider_slug: snowcap-compute
slug: snowcap-compute-domain-security
source_filename: snowcap-compute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.snowcapcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: snowcapcompute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowcap-compute/refs/heads/main/security/snowcap-compute-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Compute
- Superconducting
- Semiconductor
- Hardware
- Artificial Intelligence
- Data Center
- Deep Tech
---
