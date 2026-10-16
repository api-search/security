---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ionity.eu
  spf: true
hosts:
- cert_expires: Dec 14 07:02:03 2026 GMT
  host: ionity.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ionity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IONITY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IONITY
provider_slug: ionity
slug: ionity-domain-security
source_filename: ionity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ionity.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 07:02:03 2026 GMT\n  hsts: false\ndomains:\n- domain: ionity.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ionity/refs/heads/main/security/ionity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EVCharging
- Infrastructure
- Europe
- Mobility
---
