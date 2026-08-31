---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: touchlight.com
  spf: true
hosts:
- cert_expires: Sep 30 11:05:16 2026 GMT
  host: touchlight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Touchlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Touchlight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Touchlight
provider_slug: touchlight
slug: touchlight-domain-security
source_filename: touchlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: touchlight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:05:16 2026 GMT\n  hsts: false\ndomains:\n- domain: touchlight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/touchlight/refs/heads/main/security/touchlight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- DNA Manufacturing
- Synthetic Biology
- Gene Therapy
- Vaccines
- Contract Manufacturing
---
