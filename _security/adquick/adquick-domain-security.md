---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: adquick.com
  spf: true
hosts:
- cert_expires: Oct 10 07:22:01 2026 GMT
  host: www.adquick.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:44:36 2026 GMT
  host: docs.adquick.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:17:07 2026 GMT
  host: api.adquick.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adquick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdQuick, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AdQuick
provider_slug: adquick
slug: adquick-domain-security
source_filename: adquick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adquick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 07:22:01 2026 GMT\n  hsts: null\n- host: docs.adquick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:44:36 2026 GMT\n  hsts: null\n- host: api.adquick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:17:07 2026 GMT\n  hsts: null\ndomains:\n- domain: adquick.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adquick/refs/heads/main/security/adquick-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Advertising
- Out Of Home Advertising
- DOOH
- Programmatic Advertising
- Media Buying
- Marketing
- MCP
---
