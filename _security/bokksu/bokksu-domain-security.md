---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bokksu.com
  spf: true
hosts:
- cert_expires: Dec 12 18:39:32 2026 GMT
  host: bokksu.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bokksu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bokksu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bokksu
provider_slug: bokksu
slug: bokksu-domain-security
source_filename: bokksu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bokksu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:39:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bokksu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokksu/refs/heads/main/security/bokksu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Subscription
- Snacks
- Japan
- E-commerce
---
