---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bttcorp.com
  spf: true
hosts:
- cert_expires: Nov 17 06:18:20 2026 GMT
  host: bttcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brain Tunnelgenix Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brain Tunnelgenix Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brain Tunnelgenix Technologies
provider_slug: brain-tunnelgenix-technologies
slug: brain-tunnelgenix-technologies-domain-security
source_filename: brain-tunnelgenix-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bttcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 06:18:20 2026 GMT\n  hsts: false\ndomains:\n- domain: bttcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brain-tunnelgenix-technologies/refs/heads/main/security/brain-tunnelgenix-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Tech
- Neuroscience
- Platform
- Wellness
---
