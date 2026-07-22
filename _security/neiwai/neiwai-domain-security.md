---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heidianer.com
  spf: true
hosts:
- cert_expires: Aug 20 01:35:16 2026 GMT
  host: neiwai.heidianer.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Neiwai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for neiwai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: neiwai
provider_slug: neiwai
slug: neiwai-domain-security
source_filename: neiwai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neiwai.heidianer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 20 01:35:16 2026 GMT\n  hsts: false\ndomains:\n- domain: heidianer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neiwai/refs/heads/main/security/neiwai-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
