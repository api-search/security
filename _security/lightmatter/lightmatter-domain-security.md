---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightmatter.co
  spf: true
hosts:
- cert_expires: Sep 12 20:28:21 2026 GMT
  host: lightmatter.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightmatter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightmatter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightmatter
provider_slug: lightmatter
slug: lightmatter-domain-security
source_filename: lightmatter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightmatter.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:28:21 2026 GMT\n  hsts: false\ndomains:\n- domain: lightmatter.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightmatter/refs/heads/main/security/lightmatter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Hardware
- Photonics
- Interconnect
- Accelerator
- Optical
- Datacenter
- Co-Packaged Optics
- Silicon
---
