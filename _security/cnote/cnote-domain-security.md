---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mycnote.com
  spf: true
hosts:
- cert_expires: Nov 23 08:35:21 2026 GMT
  host: www.mycnote.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cnote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cnote, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cnote
provider_slug: cnote
slug: cnote-domain-security
source_filename: cnote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mycnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 08:35:21 2026 GMT\n  hsts: false\ndomains:\n- domain: mycnote.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnote/refs/heads/main/security/cnote-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Impact Investing
- Cash Management
- Fixed Income
- Community Development
---
