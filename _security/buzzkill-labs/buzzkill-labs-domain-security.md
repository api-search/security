---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
hosts:
- cert_expires: Dec 21 07:53:45 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buzzkill Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buzzkill Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buzzkill Labs
provider_slug: buzzkill-labs
slug: buzzkill-labs-domain-security
source_filename: buzzkill-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buzzkill-labs/refs/heads/main/security/buzzkill-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Moderation
- Sentiment
- Analytics
---
