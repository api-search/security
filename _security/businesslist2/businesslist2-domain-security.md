---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nobul.com
  spf: true
hosts:
- cert_expires: Dec 28 10:07:51 2026 GMT
  host: nobul.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Businesslist2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Businesslist2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Businesslist2
provider_slug: businesslist2
slug: businesslist2-domain-security
source_filename: businesslist2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nobul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 10:07:51 2026 GMT\n  hsts: false\ndomains:\n- domain: nobul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/businesslist2/refs/heads/main/security/businesslist2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Marketplace
- AI
- Pre-IPO
- Investment
---
