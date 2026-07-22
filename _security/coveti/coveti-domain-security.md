---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coveti.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: coveti.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coveti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coveti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coveti
provider_slug: coveti
slug: coveti-domain-security
source_filename: coveti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coveti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: coveti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coveti/refs/heads/main/security/coveti-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fashion
- Luxury
- Marketplace
- Ecommerce
- Retail
- Agentic Commerce
- AI Styling
---
