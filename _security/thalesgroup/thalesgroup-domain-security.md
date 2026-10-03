---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thalesgroup.com
  spf: true
hosts:
- cert_expires: Nov 24 19:35:22 2026 GMT
  host: www.thalesgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thalesgroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Thales
provider_slug: thalesgroup
slug: thalesgroup-domain-security
source_filename: thalesgroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thalesgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 19:35:22 2026 GMT\n  hsts: false\ndomains:\n- domain: thalesgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thalesgroup/refs/heads/main/security/thalesgroup-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Technology
- Aerospace
- Defense
- DigitalIdentity
---
