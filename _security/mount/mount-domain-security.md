---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mount.insure
  spf: true
hosts:
- cert_expires: Aug 26 17:09:29 2026 GMT
  host: mount.insure
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mount Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mount, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mount
provider_slug: mount
slug: mount-domain-security
source_filename: mount-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mount.insure\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mount.insure\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mount/refs/heads/main/security/mount-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Artificial Intelligence
- AI Agents
- AI Safety
- Risk
- Security
- Y Combinator
---
