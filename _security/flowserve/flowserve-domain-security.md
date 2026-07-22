---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: flowserve.com
  spf: true
hosts:
- cert_expires: Sep 15 12:53:19 2026 GMT
  host: www.flowserve.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowserve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Flowserve
provider_slug: flowserve
slug: flowserve-domain-security
source_filename: flowserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flowserve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:53:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: flowserve.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowserve/refs/heads/main/security/flowserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Industrial
- Flow Control
- IIoT
- Manufacturing
- Fortune 1000
---
