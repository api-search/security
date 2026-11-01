---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mewe.com
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: mewe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mewe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeWe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MeWe
provider_slug: mewe
slug: mewe-domain-security
source_filename: mewe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mewe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mewe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mewe/security/mewe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social
- Privacy
- Networking
- Communication
---
