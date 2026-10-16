---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crowdgen.com
  spf: true
hosts:
- cert_expires: Dec 17 11:04:36 2026 GMT
  host: crowdgen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowdflower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdflower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crowdflower
provider_slug: crowdflower
slug: crowdflower-domain-security
source_filename: crowdflower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 11:04:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crowdgen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdflower/refs/heads/main/security/crowdflower-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- AI
- Crowdsourcing
- Marketplace
---
