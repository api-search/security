---
api_specs:
- filename: 4k-garden-diebian-ai-openapi.json
  format: json
  label: Diebian AI Super-Resolution API
  slug: diebian-ai-super-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-diebian-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 4kgarden.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fly4k.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.4kgarden.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.fly4k.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: video-cn.fly4k.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 4K Garden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4K Garden, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 4K Garden
provider_slug: 4k-garden
slug: 4k-garden-domain-security
source_filename: 4k-garden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4kgarden.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: www.fly4k.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\n- host: video-cn.fly4k.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 4kgarden.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fly4k.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/security/4k-garden-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Video
- Ultra High Definition
- Media and Entertainment
- Content Distribution
- Live Streaming
- Artificial Intelligence
- Video Super Resolution
- Virtual Reality
- China
---
