---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abcommunity.org
  spf: true
hosts:
- cert_expires: Dec 13 10:19:10 2026 GMT
  host: abcommunity.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Builders Community Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Builders Community, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Builders Community
provider_slug: abcommunity-org
slug: abcommunity-org-domain-security
source_filename: abcommunity-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcommunity.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:19:10 2026 GMT\n  hsts: false\ndomains:\n- domain: abcommunity.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/abcommunity-org/security/abcommunity-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Community
- Builders
- Azerbaijan
- Platform
---
