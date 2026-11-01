---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fes.org.in
  spf: true
hosts:
- cert_expires: Dec 22 10:51:55 2026 GMT
  host: www.fes.org.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foundation For Ecological Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundation for Ecological Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Foundation for Ecological Security
provider_slug: foundation-for-ecological-security
slug: foundation-for-ecological-security-domain-security
source_filename: foundation-for-ecological-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fes.org.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 10:51:55 2026 GMT\n  hsts: false\ndomains:\n- domain: fes.org.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foundation-for-ecological-security/security/foundation-for-ecological-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Nonprofit
- Environment
- Conservation
- Climate
- India
---
