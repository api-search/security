---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: with.us
  spf: false
hosts:
- cert_expires: Oct 10 23:30:22 2026 GMT
  host: with.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Withco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Withco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Withco
provider_slug: withco
slug: withco-domain-security
source_filename: withco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: with.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:30:22 2026 GMT\n  hsts: false\ndomains:\n- domain: with.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withco/refs/heads/main/security/withco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Small Business
- Commercial Real Estate
- Investing
- Community Ownership
- Main Street
---
