---
description: ''
domains:
- caa:
  - m.geetest.com.w.alikunlun.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: geetest.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: geetest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geetest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeeTest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GeeTest
provider_slug: geetest
slug: geetest-domain-security
source_filename: geetest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geetest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: geetest.com\n  dnssec: true\n  caa:\n  - m.geetest.com.w.alikunlun.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/geetest/security/geetest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Security
- BotManagement
- CAPTCHA
- FraudPrevention
- Enterprise
---
