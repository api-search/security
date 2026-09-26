---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: audion.com
  spf: true
hosts:
- cert_expires: Nov 28 16:04:39 2026 GMT
  host: www.audion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Audion
provider_slug: audion
slug: audion-domain-security
source_filename: audion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.audion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:04:39 2026 GMT\n  hsts: false\ndomains:\n- domain: audion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audion/refs/heads/main/security/audion-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Packaging
- Manufacturing
- Automation
- Sustainability
---
