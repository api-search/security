---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: buzz360.co
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.buzz360.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buzz360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buzz360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Buzz360
provider_slug: buzz360
slug: buzz360-domain-security
source_filename: buzz360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buzz360.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: buzz360.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buzz360/refs/heads/main/security/buzz360-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Political
- CampaignSoftware
- VoterEngagement
- CRM
- Conservative
---
