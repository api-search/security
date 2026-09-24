---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: leaf.space
  spf: true
hosts:
- cert_expires: Oct 28 14:31:47 2026 GMT
  host: leaf.space
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leaf Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaf Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Leaf Space
provider_slug: leaf-space
slug: leaf-space-domain-security
source_filename: leaf-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leaf.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 14:31:47 2026 GMT\n  hsts: false\ndomains:\n- domain: leaf.space\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaf-space/refs/heads/main/security/leaf-space-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Satellite
- Connectivity
- GroundStation
- Space
---
