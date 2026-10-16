---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brilliant.org
  spf: true
hosts:
- cert_expires: Dec 14 10:00:48 2026 GMT
  host: brilliant.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brilliantdotorg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brilliantdotorg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brilliantdotorg
provider_slug: brilliantdotorg
slug: brilliantdotorg-domain-security
source_filename: brilliantdotorg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brilliant.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 10:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: brilliant.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brilliantdotorg/refs/heads/main/security/brilliantdotorg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
