---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ehalsomyndigheten.se
  spf: true
hosts:
- cert_expires: Dec 25 16:18:50 2026 GMT
  host: www.ehalsomyndigheten.se
  hsts: true
  hsts_max_age: 11664000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ehalsomyndigheten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for E-halsomyndigheten (Swedish eHealth Agency), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: E-halsomyndigheten (Swedish eHealth Agency)
provider_slug: ehalsomyndigheten
slug: ehalsomyndigheten-domain-security
source_filename: ehalsomyndigheten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ehalsomyndigheten.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 16:18:50 2026 GMT\n  hsts: true\n  hsts_max_age: 11664000\ndomains:\n- domain: ehalsomyndigheten.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ehalsomyndigheten/refs/heads/main/security/ehalsomyndigheten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- eHealth
- Sweden
- Government
- DigitalHealth
---
