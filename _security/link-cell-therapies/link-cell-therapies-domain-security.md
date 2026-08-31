---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: linkcelltx.com
  spf: true
hosts:
- cert_expires: Sep 30 08:19:46 2026 GMT
  host: linkcelltx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Link Cell Therapies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Link Cell Therapies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Link Cell Therapies
provider_slug: link-cell-therapies
slug: link-cell-therapies-domain-security
source_filename: link-cell-therapies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkcelltx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:19:46 2026 GMT\n  hsts: false\ndomains:\n- domain: linkcelltx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/link-cell-therapies/refs/heads/main/security/link-cell-therapies-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- CAR T
- Oncology
- Immunotherapy
- Precision Medicine
- Clinical Stage
---
