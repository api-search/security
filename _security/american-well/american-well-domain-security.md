---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amwell.com
  spf: true
hosts:
- cert_expires: Nov 10 20:59:15 2026 GMT
  host: business.amwell.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: American Well Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Well, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: American Well
provider_slug: american-well
slug: american-well-domain-security
source_filename: american-well-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.amwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 20:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: amwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-well/refs/heads/main/security/american-well-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
