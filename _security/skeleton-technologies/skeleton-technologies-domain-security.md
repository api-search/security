---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skeletontech.com
  spf: true
hosts:
- cert_expires: Nov 17 21:43:37 2026 GMT
  host: www.skeletontech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skeleton Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skeleton Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Skeleton Technologies
provider_slug: skeleton-technologies
slug: skeleton-technologies-domain-security
source_filename: skeleton-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skeletontech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 21:43:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skeletontech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skeleton-technologies/refs/heads/main/security/skeleton-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy Storage
- Supercapacitors
- Ultracapacitors
- Graphene
- Manufacturing
- Data Centers
- Grid Stability
- Hardware
- Estonia
- Germany
---
