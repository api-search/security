---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cgzair.com
  spf: true
hosts:
- cert_expires: Dec 21 07:53:45 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.cgzair.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Colorful Guizhou Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colorful Guizhou Airlines, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Colorful Guizhou Airlines
provider_slug: colorful-guizhou-airlines
slug: colorful-guizhou-airlines-domain-security
source_filename: colorful-guizhou-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cgzair.com\n  https: false\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cgzair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorful-guizhou-airlines/refs/heads/main/security/colorful-guizhou-airlines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- airline
- china
- low-cost
- regional
- guizhou
---
