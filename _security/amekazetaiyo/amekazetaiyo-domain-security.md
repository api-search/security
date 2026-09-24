---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ame-kaze-taiyo.jp
  spf: true
hosts:
- cert_expires: Nov 17 09:13:05 2026 GMT
  host: ame-kaze-taiyo.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amekazetaiyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amekazetaiyo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amekazetaiyo
provider_slug: amekazetaiyo
slug: amekazetaiyo-domain-security
source_filename: amekazetaiyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ame-kaze-taiyo.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 09:13:05 2026 GMT\n  hsts: false\ndomains:\n- domain: ame-kaze-taiyo.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amekazetaiyo/refs/heads/main/security/amekazetaiyo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Japan
- UrbanRural
- Community
- Services
---
