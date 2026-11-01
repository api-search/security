---
description: ''
domains:
- caa:
  - leadmaster-aii.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: false
  dnssec: true
  domain: minaxlab.com
  spf: true
hosts:
- cert_expires: Dec 12 09:15:16 2026 GMT
  host: minaxlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Minaxlab Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for minaxlab-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: minaxlab-com
provider_slug: minaxlab-com
slug: minaxlab-com-domain-security
source_filename: minaxlab-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minaxlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 09:15:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minaxlab.com\n  dnssec: true\n  caa:\n  - leadmaster-aii.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/minaxlab-com/security/minaxlab-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- AI
- Creative
- Tools
- Platform
---
