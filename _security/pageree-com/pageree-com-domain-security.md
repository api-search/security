---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pageree.com
  spf: true
hosts:
- cert_expires: Feb  3 10:31:17 2027 GMT
  host: pageree.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pageree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pageree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pageree
provider_slug: pageree-com
slug: pageree-com-domain-security
source_filename: pageree-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pageree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 10:31:17 2027 GMT\n  hsts: false\ndomains:\n- domain: pageree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pageree-com/security/pageree-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI landing page builder
- Lead Capture
- First‑party analytics
- ChatGPT integration
- No‑code publishing
- Software-as-a-Service
---
