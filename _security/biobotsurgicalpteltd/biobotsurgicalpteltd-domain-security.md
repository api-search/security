---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biobotsurgical.com
  spf: true
hosts:
- cert_expires: Dec  4 11:22:10 2026 GMT
  host: biobotsurgical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biobotsurgicalpteltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biobotsurgicalpteltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biobotsurgicalpteltd
provider_slug: biobotsurgicalpteltd
slug: biobotsurgicalpteltd-domain-security
source_filename: biobotsurgicalpteltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biobotsurgical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 11:22:10 2026 GMT\n  hsts: false\ndomains:\n- domain: biobotsurgical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biobotsurgicalpteltd/refs/heads/main/security/biobotsurgicalpteltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical
- Robotics
- Healthcare
- Singapore
---
