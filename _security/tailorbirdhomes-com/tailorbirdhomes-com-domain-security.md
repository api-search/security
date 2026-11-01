---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tailorbirdhomes.com
  spf: true
hosts:
- cert_expires: Jan  9 16:40:40 2027 GMT
  host: www.tailorbirdhomes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tailorbirdhomes Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailorbird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tailorbird
provider_slug: tailorbirdhomes-com
slug: tailorbirdhomes-com-domain-security
source_filename: tailorbirdhomes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tailorbirdhomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:40:40 2027 GMT\n  hsts: null\ndomains:\n- domain: tailorbirdhomes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tailorbirdhomes-com/security/tailorbirdhomes-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- RealEstate
- CapEx
- AI
- PropertyData
---
